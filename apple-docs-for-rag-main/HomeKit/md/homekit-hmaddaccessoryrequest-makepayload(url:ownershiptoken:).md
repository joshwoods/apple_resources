

- HomeKit
- HMAddAccessoryRequest
-  makePayload(url:ownershipToken:) 

Instance Method

# makePayload(url:ownershipToken:)

Builds an accessory setup payload with the given setup payload URL and ownership token.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
func makePayload(
    url setupPayloadURL: URL,
    ownershipToken: HMAccessoryOwnershipToken
) -> HMAccessorySetupPayload?
```

## Parameters 

`setupPayloadURL`  

The setup payload URL for the accessory. Provide this URL when HomeKit sends an add request to the app associated with your accessory. You determine the URL based on the category and name of your accessory, as given in the accessoryCategory and accessoryName properties of the associated HMAddAccessoryRequest instance.

`ownershipToken`  

A token proving ownership of the accessory. Your app negotiates the token with the accessory outside of HomeKit.

## Return Value

An accessory setup payload that you use to add the accessory. The method fails and returns `nil` if the setup payload URL is invalid.

## See Also

### Creating a Payload

func makePayload(ownershipToken: HMAccessoryOwnershipToken) -> HMAccessorySetupPayload?

Builds an accessory setup payload with the given ownership token.

