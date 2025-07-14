

- PassKit (Apple Pay and Wallet)
- PKAddIdentityDocumentConfiguration
-  metadata 

Instance Property

# metadata

A set of configurable metadata that defines the required information to add the corresponding pass to Wallet.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
var metadata: PKIdentityDocumentMetadata { get }
```

## See Also

### Setting the metadata

class func forMetadata(PKIdentityDocumentMetadata, completion: (PKAddIdentityDocumentConfiguration?, (any Error)?) -> Void)

Returns the identity document configuration.

