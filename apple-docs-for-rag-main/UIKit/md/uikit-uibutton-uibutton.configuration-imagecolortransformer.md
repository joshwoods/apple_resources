

- UIKit
- UIButton
- UIButton.Configuration
-  imageColorTransformer 

Instance Property

# imageColorTransformer

A block that transforms the image color when the button state changes.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var imageColorTransformer: UIConfigurationColorTransformer? { get set }
```

## Discussion

Use this property to transform an image to, for example, a monochrome or tinted image.

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

var preferredSymbolConfigurationForImage: UIImage.SymbolConfiguration?

A requested configuration object for the button symbol image.

