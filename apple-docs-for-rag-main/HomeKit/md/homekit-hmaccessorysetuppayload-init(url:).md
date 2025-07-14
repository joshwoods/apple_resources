

- HomeKit
- HMAccessorySetupPayload
-  init(url:) 

Initializer

# init(url:)

Creates an accessory setup payload.

iOS 11.3+iPadOS 11.3+visionOS 1.0+

``` source
init?(url setupPayloadURL: URL?)
```

## Parameters 

`setupPayloadURL`  

The payload used to securely authenticate the accessory. This is the same payload you would receive by scanning the accessory’s QR code.

## Discussion

For details about the payload’s content, please join the MFi Program.

## See Also

### Creating a Payload

init?(url: URL, ownershipToken: HMAccessoryOwnershipToken?)

Creates an accessory setup payload instance that includes an ownership token.

class HMAccessoryOwnershipToken

Authentication data that your app provides when adding an accessory to a home.

