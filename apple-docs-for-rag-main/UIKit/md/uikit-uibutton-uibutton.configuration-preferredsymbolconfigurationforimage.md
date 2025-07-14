

- UIKit
- UIButton
- UIButton.Configuration
-  preferredSymbolConfigurationForImage 

Instance Property

# preferredSymbolConfigurationForImage

A requested configuration object for the button symbol image.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var preferredSymbolConfigurationForImage: UIImage.SymbolConfiguration? { get set }
```

## Discussion

A symbol configuration defines details such as the point size, scale, text style, weight, and font of symbol image. The button uses these details to determine which variant of the image to use and how to scale or style the image.

## See Also

### Configuring images

var image: UIImage?

The foreground image the button displays.

var imagePadding: CGFloat

The distance between the button’s image and text.

var imagePlacement: NSDirectionalRectEdge

The edge against which the button places the image.

var imageReservation: CGFloat

A value that reserves space for the image in the same axis as the edge against which the button places the image.

var imageColorTransformer: UIConfigurationColorTransformer?

A block that transforms the image color when the button state changes.

