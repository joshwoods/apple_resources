

- HomeKit
-  HMAccessorySetupPayload 

Class

# HMAccessorySetupPayload

A payload for authenticating a HomeKit accessory.

iOS 11.3+iPadOS 11.3+visionOS 1.0+

``` source
class HMAccessorySetupPayload
```

## Overview

The setup payload provides a URL to authenticate an accessory. Typically, the URL comes from scanning a QR code on the accessory. Use a setup payload to authenticate devices that are already deployed, for which scanning a QR code would be difficult, or if you need to provide an optional ownership token that you negotiate with the accessory outside of HomeKit.

For details about the payload’s content, please join the MFi Program.

## Topics

### Creating a Payload

init?(url: URL?)

Creates an accessory setup payload.

init?(url: URL, ownershipToken: HMAccessoryOwnershipToken?)

Creates an accessory setup payload instance that includes an ownership token.

class HMAccessoryOwnershipToken

Authentication data that your app provides when adding an accessory to a home.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

