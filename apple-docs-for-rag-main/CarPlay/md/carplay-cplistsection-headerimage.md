

- CarPlay
- CPListSection
-  headerImage 

Instance Property

# headerImage

An image that the section header displays.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@NSCopying
var headerImage: UIImage? { get set }
```

## Discussion

The maximum size of the section header image is CPMaximumListSectionImageSize.

Provide a UIImage that is display-ready. To provide an image that includes light and dark styles, use an asset from your asset catalog that includes both styles, or use a UIImageAsset to combine two UIImage instances into a single image with both styles.

To size your header image properly, consider the display scale of the car screen. Use UIImageAsset to combine multiple images with different trait collections into a single image. For more information about trait collections for CarPlay, see carTraitCollection.

## See Also

### Configuring Section Headers

var headerButton: CPButton?

A button that the section header displays.

var headerSubtitle: String?

A string that the header displays as a subtitle.

