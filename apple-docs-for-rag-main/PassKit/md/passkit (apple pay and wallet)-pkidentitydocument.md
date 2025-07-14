

- PassKit (Apple Pay and Wallet)
-  PKIdentityDocument 

Class

# PKIdentityDocument

An object that represents the response to a request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class PKIdentityDocument
```

## Mentioned in 

Requesting identity data from a Wallet pass

## Topics

### Configuring an identity document

var encryptedData: Data

An encrypted data object that contains the document information and metadata to associate with a request.

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

## See Also

### Identity sheet interactions and authorization

Requesting identity data from a Wallet pass

Initiate a request for identity information by prompting a user for permission and decrypting a response payload.

Verifying Wallet identity requests

Decrypt and verify an in-app presentment request on your server.

class PKIdentityAuthorizationController

An object that presents a sheet that prompts the user to allow a request for identity information.

class PKIdentityRequest

An object that represents a request for identity information from a Wallet pass.

class PKIdentityElement

An object that represents the elements an app requests from identity documents.

class PKIdentityButton

An object that displays a button to trigger the identity verification flow.

struct VerifyIdentityWithWalletButton

A view that displays a button for identity verification.

struct VerifyIdentityWithWalletButtonLabel

A type that represents the label you use with a verify identity button.

struct VerifyIdentityWithWalletButtonStyle

A type that represents the style you use with a verify identity button.

