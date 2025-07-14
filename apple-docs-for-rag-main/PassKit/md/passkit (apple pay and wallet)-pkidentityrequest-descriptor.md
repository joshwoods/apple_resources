

- PassKit (Apple Pay and Wallet)
- PKIdentityRequest
-  descriptor 

Instance Property

# descriptor

The description of the document the app requests.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
var descriptor: (any PKIdentityDocumentDescriptor)? { get set }
```

## Discussion

Set this property before you invoke requestDocument(_:completion:).

## See Also

### Configuring an identity request

var nonce: Data?

An arbitrary number that the signed response playload includes.

var merchantIdentifier: String?

A value that represents the merchant that makes the request.

