

- PassKit (Apple Pay and Wallet)
- PKAddPassMetadataPreview
-  init(passThumbnail:localizedDescription:) 

Initializer

# init(passThumbnail:localizedDescription:)

Provides a preview of an image object that represents the pass you add to Wallet.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
init(
    passThumbnail: CGImage,
    localizedDescription description: String
)
```

## Parameters 

`passThumbnail`  

A CGImage object that represents the card artwork of the pass you use during provisioning.

`description`  

A localized description of the pass.

## Discussion

This method throws an `invalidInput` error if a JPKI applet doesn’t back the pass.

## See Also

### Creating a preview of the pass

var localizedDescription: String?

A localized description of the pass.

var passThumbnailImage: CGImage?

A CGImage object representing the card artwork of the pass you use during provisioning.

