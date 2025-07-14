

- PassKit (Apple Pay and Wallet)
- PKIdentityRequest
-  nonce 

Instance Property

# nonce

An arbitrary number that the signed response playload includes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
var nonce: Data? { get set }
```

## Mentioned in 

Requesting identity data from a Wallet pass

Verifying Wallet identity requests

## Discussion

A PKIdentityAuthorizationController treats this value as opaque, and has a maximum allowed size of 64 bytes. Your app’s server needs to use the same `nonce` value when decrypting and verifying the response.

Set this property before you invoke requestDocument(_:completion:).

## See Also

### Configuring an identity request

var descriptor: (any PKIdentityDocumentDescriptor)?

The description of the document the app requests.

var merchantIdentifier: String?

A value that represents the merchant that makes the request.

