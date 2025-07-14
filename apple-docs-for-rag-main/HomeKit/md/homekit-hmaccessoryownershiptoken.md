

- HomeKit
-  HMAccessoryOwnershipToken 

Class

# HMAccessoryOwnershipToken

Authentication data that your app provides when adding an accessory to a home.

iOS 13.0+iPadOS 13.0+visionOS 1.0+

``` source
class HMAccessoryOwnershipToken
```

## Overview

If you manufacture an accessory that requires user authentication to add the accessory to a home, manage the authentication in your app and produce a token that represents the successful outcome of that process. Wrap the token data in an HMAccessoryOwnershipToken instance and call the init(url:ownershipToken:) method to create an authenticated HMAccessorySetupPayload instance. Then call the addAndSetupAccessories(with:completionHandler:) method with the payload.

If the user attempts from the Home app to add an accessory that requires a token, the Home app calls the associated app’s homeManager(_:didReceiveAddAccessoryRequest:) home manager delegate method to perform the negotiation and provide the token.

## Topics

### Creating a Token

init?(data: Data)

Creates an ownership token from data.

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

## See Also

### Creating a Payload

init?(url: URL?)

Creates an accessory setup payload.

init?(url: URL, ownershipToken: HMAccessoryOwnershipToken?)

Creates an accessory setup payload instance that includes an ownership token.

