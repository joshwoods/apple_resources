

- HomeKit
- HMHomeManagerDelegate
-  homeManager(\_:didReceiveAddAccessoryRequest:) 

Instance Method

# homeManager(\_:didReceiveAddAccessoryRequest:)

Tells the delegate to add an accessory to a home by using a setup payload.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
optional func homeManager(
    _ manager: HMHomeManager,
    didReceiveAddAccessoryRequest request: HMAddAccessoryRequest
)
```

## Parameters 

`manager`  

The home manager making the request.

`request`  

A description of the accessory to add.

## Discussion

HomeKit calls this method when it needs help adding an accessory to a home, which typically occurs when the accessory requires explicit user authentication that HomeKit can’t negotiate. HomeKit asks the accessory manufacturer’s app, which it locates using information provided by the accessory, to complete the authentication.

If you manufacture an accessory like this, handle the homeManager(_:didReceiveAddAccessoryRequest:) call in your app by creating an HMAccessoryOwnershipToken instance in a way that’s appropriate for your accessory, outside of HomeKit:

```
let data = negotiateTokenData(accessory: request.accessoryName)
guard let token = HMAccessoryOwnershipToken(data: data) else { return }
```

Use the resulting token to create an HMAccessorySetupPayload instance. If the request’s requiresSetupPayloadURL flag is `true`, get the payload URL corresponding to the named accessory, and include that in the setup payload as well:

```
var payload: HMAccessorySetupPayload?
if request.requiresSetupPayloadURL {
    let payloadURL = getPayloadURL(accessory: request.accessoryName)
    payload = request.makePayload(url: payloadURL, ownershipToken: token)
} else {
    payload = request.makePayload(ownershipToken: token)
}
```

Complete the setup by calling the home’s addAndSetupAccessories(with:completionHandler:) method with the payload:

```
if let payload = payload {
    request.home.addAndSetupAccessories(with: payload) { accessories, error in
        // Handle errors.
    }
}
```

## See Also

### Adding accessories

class HMAddAccessoryRequest

A request to add an accessory to a particular home.

