

- HomeKit
- HMAccessorySetupPayload
-  init(url:ownershipToken:) 

Initializer

# init(url:ownershipToken:)

Creates an accessory setup payload instance that includes an ownership token.

iOS 13.0+iPadOS 13.0+visionOS 1.0+

``` source
init?(
    url setupPayloadURL: URL,
    ownershipToken: HMAccessoryOwnershipToken?
)
```

## Parameters 

`setupPayloadURL`  

The payload used to securely authenticate the accessory. This is the same payload you would receive by scanning the accessory’s QR code.

`ownershipToken`  

A token that proves ownership of the accessory. You typically negotiate this token with the accessory outside of HomeKit.

## Discussion

For details about the payload’s content, join the MFi Program.

## See Also

### Creating a Payload

init?(url: URL?)

Creates an accessory setup payload.

class HMAccessoryOwnershipToken

Authentication data that your app provides when adding an accessory to a home.

