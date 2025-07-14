

- UIKit
- UIButton
- UIButton.Configuration
-  imagePlacement 

Instance Property

# imagePlacement

The edge against which the button places the image.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var imagePlacement: NSDirectionalRectEdge { get set }
```

## Discussion

Use this property to place the image along the top, leading, trailing, or bottom edge of the button.

## See Also

### Configuring images

var image: UIImage?

The foreground image the button displays.

var imagePadding: CGFloat

The distance between the button’s image and text.

var imageReservation: CGFloat

A value that reserves space for the image in the same axis as the edge against which the button places the image.

var imageColorTransformer: UIConfigurationColorTransformer?

A block that transforms the image color when the button state changes.

var preferredSymbolConfigurationForImage: UIImage.SymbolConfiguration?

A requested configuration object for the button symbol image.

