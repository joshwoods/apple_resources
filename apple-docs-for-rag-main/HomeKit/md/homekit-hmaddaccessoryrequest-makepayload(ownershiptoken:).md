

- HomeKit
- HMAddAccessoryRequest
-  makePayload(ownershipToken:) 

Instance Method

# makePayload(ownershipToken:)

Builds an accessory setup payload with the given ownership token.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
func makePayload(ownershipToken: HMAccessoryOwnershipToken) -> HMAccessorySetupPayload?
```

## Parameters 

`ownershipToken`  

A token proving ownership of the accessory.

## Return Value

An accessory setup payload that you use to add the accessory. The method fails and returns `nil` if the request’s requiresSetupPayloadURL property is `true`. In that case, use makePayload(url:ownershipToken:) instead.

## See Also

### Creating a Payload

func makePayload(url: URL, ownershipToken: HMAccessoryOwnershipToken) -> HMAccessorySetupPayload?

Builds an accessory setup payload with the given setup payload URL and ownership token.

