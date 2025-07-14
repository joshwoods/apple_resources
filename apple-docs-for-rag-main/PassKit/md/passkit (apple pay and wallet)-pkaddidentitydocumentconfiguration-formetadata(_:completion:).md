

- PassKit (Apple Pay and Wallet)
- PKAddIdentityDocumentConfiguration
-  forMetadata(\_:completion:) 

Type Method

# forMetadata(\_:completion:)

Returns the identity document configuration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
class func forMetadata(
    _ metadata: PKIdentityDocumentMetadata,
    completion: @escaping (PKAddIdentityDocumentConfiguration?, (any Error)?) -> Void
)
```

``` source
class func forMetadata(_ metadata: PKIdentityDocumentMetadata) async throws -> PKAddIdentityDocumentConfiguration
```

## Parameters 

`metadata`  

The configurable metadata that defines the required information to add the corresponding pass to Wallet.

`completion`  

Returns the identity document configration.

## See Also

### Setting the metadata

var metadata: PKIdentityDocumentMetadata

A set of configurable metadata that defines the required information to add the corresponding pass to Wallet.

