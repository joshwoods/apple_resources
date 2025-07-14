

- UIKit
- UIButton
- UIButton.Configuration
-  imageReservation 

Instance Property

# imageReservation

A value that reserves space for the image in the same axis as the edge against which the button places the image.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var imageReservation: CGFloat { get set }
```

## Discussion

Defaults to `0`. The value reserves space in the axis that corresponds to imagePlacement. If the image is larger than the reservation value in that axis, the system ignores the reservation value. Otherwise, the system centers the image in the space that the reservation value provides.

If the image is a symbol image, the system scales the reservation value with dynamic type, based on the image configuration.

## See Also

### Configuring images

var image: UIImage?

The foreground image the button displays.

var imagePadding: CGFloat

The distance between the button’s image and text.

var imagePlacement: NSDirectionalRectEdge

The edge against which the button places the image.

var imageColorTransformer: UIConfigurationColorTransformer?

A block that transforms the image color when the button state changes.

var preferredSymbolConfigurationForImage: UIImage.SymbolConfiguration?

A requested configuration object for the button symbol image.

