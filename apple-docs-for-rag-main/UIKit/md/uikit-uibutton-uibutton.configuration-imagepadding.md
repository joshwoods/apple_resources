

- UIKit
- UIButton
- UIButton.Configuration
-  imagePadding 

Instance Property

# imagePadding

The distance between the button’s image and text.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var imagePadding: CGFloat { get set }
```

## Discussion

Use this property to adjust the distance from the title and subtitle. This doesn’t affect the distance to the button’s edge.

## See Also

### Configuring images

var image: UIImage?

The foreground image the button displays.

var imagePlacement: NSDirectionalRectEdge

The edge against which the button places the image.

var imageReservation: CGFloat

A value that reserves space for the image in the same axis as the edge against which the button places the image.

var imageColorTransformer: UIConfigurationColorTransformer?

A block that transforms the image color when the button state changes.

var preferredSymbolConfigurationForImage: UIImage.SymbolConfiguration?

A requested configuration object for the button symbol image.

