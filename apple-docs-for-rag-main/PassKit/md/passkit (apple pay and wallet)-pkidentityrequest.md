

- PassKit (Apple Pay and Wallet)
-  PKIdentityRequest 

Class

# PKIdentityRequest

An object that represents a request for identity information from a Wallet pass.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class PKIdentityRequest
```

## Mentioned in 

Verifying Wallet identity requests

## Overview

A request consists of a PKIdentityDocumentDescriptor, a nonce, and a merchantIdentifier. A PKIdentityDocumentDescriptor describes the document an app requests.

You use a nonce to verify a request is only made once. It’s up to the app and its server to generate the nonce before making the request, and to verify the nonce when the server receives the response.

The merchantIdentifier maps to an identifier you configure in the developer portal. Payment and identitity requests share the same identifier, so it’s important that the name of the property matches the equivalent PKPaymentRequest, if necessary.

## Topics

### Configuring an identity request

var descriptor: (any PKIdentityDocumentDescriptor)?

The description of the document the app requests.

var nonce: Data?

An arbitrary number that the signed response playload includes.

var merchantIdentifier: String?

A value that represents the merchant that makes the request.

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

class PKIdentityDocument

An object that represents the response to a request.

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

