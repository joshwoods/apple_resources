

- PassKit (Apple Pay and Wallet)
-  PKIdentityAuthorizationController 

Class

# PKIdentityAuthorizationController

An object that presents a sheet that prompts the user to allow a request for identity information.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class PKIdentityAuthorizationController
```

## Mentioned in 

Requesting identity data from a Wallet pass

## Overview

Use this class to request PKIdentityElement objects from a mobile driver’s license or state identification card. When you request identity information, the system prompts the user for approval.

```
// Create an authorization controller.
let controller = PKIdentityAuthorizationController()

// Describe the elements you request.
let descriptor = PKIdentityDriversLicenseDescriptor()
descriptor.addElements([.age(atLeast: 18)], 
                        intentToStore: .willNotStore)
descriptor.addElements([.givenName, .portrait], 
                        intentToStore: .mayStore(days: 30))

// Create the request.
let request = PKIdentityRequest()
request.descriptor = descriptor
request.merchantIdentifier = // A merchant identifier you configure in the developer portal.
request.nonce = // Generate a nonce to verify a request is only made once.

// Prompt the user for approval.
controller.requestDocument(request) { document, error in
    // Handle the document response or error, if necessary.
}
```

The system returns response data as an encoded concise binary object representation (CBOR) blob; CBOR is a binary format similar to JSON. You must decrypt the response on your server.

For design guidance, see Human Interface Guidelines > Technologies > Wallet.

Important

This API only works on iPhone and returns an error if you access it on iPad. This framework requires a special entitlement from Apple. This entitlement is not yet available.

## Topics

### Describing a document

class PKIdentityDriversLicenseDescriptor

An object for requesting information from a user’s driver’s license or equivalent document.

class PKIdentityIntentToStore

An object that represents your intention to store an identity element or values derived from an identity element.

protocol PKIdentityDocumentDescriptor

A type that describes the structure and behavior of an identity document.

### Requesting a document

func checkCanRequestDocument(any PKIdentityDocumentDescriptor, completion: (Bool) -> Void)

Returns whether an identity document is available to request.

func requestDocument(PKIdentityRequest, completion: (PKIdentityDocument?, (any Error)?) -> Void)

Prompts the user to approve the request to get the identity information.

### Cancelling a request

func cancelRequest()

Cancels a request in progress.

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

class PKIdentityRequest

An object that represents a request for identity information from a Wallet pass.

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

