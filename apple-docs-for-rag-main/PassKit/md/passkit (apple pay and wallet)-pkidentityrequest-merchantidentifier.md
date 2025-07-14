

- PassKit (Apple Pay and Wallet)
- PKIdentityRequest
-  merchantIdentifier 

Instance Property

# merchantIdentifier

A value that represents the merchant that makes the request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
var merchantIdentifier: String? { get set }
```

## Discussion

This property identifies the merchant making the request, and must match one of the merchant identifiers in the app’s entitlement. For information about configuring the entitlement, see com.apple.developer.in-app-identity-presentment.merchant-identifiers.

Set this property before you invoke requestDocument(_:completion:).

## See Also

### Configuring an identity request

var descriptor: (any PKIdentityDocumentDescriptor)?

The description of the document the app requests.

var nonce: Data?

An arbitrary number that the signed response playload includes.

