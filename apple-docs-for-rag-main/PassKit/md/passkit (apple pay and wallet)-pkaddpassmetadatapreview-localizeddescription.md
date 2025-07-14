

- PassKit (Apple Pay and Wallet)
- PKAddPassMetadataPreview
-  localizedDescription 

Instance Property

# localizedDescription

A localized description of the pass.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
var localizedDescription: String? { get }
```

## See Also

### Creating a preview of the pass

init(passThumbnail: CGImage, localizedDescription: String)

Provides a preview of an image object that represents the pass you add to Wallet.

var passThumbnailImage: CGImage?

A CGImage object representing the card artwork of the pass you use during provisioning.

