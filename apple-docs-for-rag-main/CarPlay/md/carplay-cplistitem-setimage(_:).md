

- CarPlay
- CPListItem
-  setImage(\_:) 

Instance Method

# setImage(\_:)

Updates the list item’s image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func setImage(_ image: UIImage?)
```

## Parameters 

`image`  

The image to display in the item’s leading region.

## Discussion

Provide an image that is display-ready. If necessary, provide light and dark variants using an asset catalog, or use an instance of UIImageAsset and register an image for each interface style. To properly size your image, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property. At runtime, use maximumImageSize to determine the maximum size for a list item’s image.

CarPlay doesn’t support animated images. If you provide an animated image, CarPlay uses only the first image in the animation sequence.

## See Also

### Managing Content

var text: String?

The list item’s primary text.

func setText(String)

Updates the list item’s primary text.

var detailText: String?

The list item’s secondary text.

func setDetailText(String?)

Updates the list item’s secondary text.

var image: UIImage?

The image that the list item displays in its leading region.

class var maximumImageSize: CGSize

The maximum size of a list item’s image and accessory image.

