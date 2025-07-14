

- UIKit
- UIButton
- UIButton.Configuration
-  image 

Instance Property

# image

The foreground image the button displays.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var image: UIImage? { get set }
```

## Discussion

A configuration contains one image. To change the image based on button state, use configurationUpdateHandler or updateConfiguration().

## See Also

### Configuring images

var imagePadding: CGFloat

The distance between the button’s image and text.

var imagePlacement: NSDirectionalRectEdge

The edge against which the button places the image.

var imageReservation: CGFloat

A value that reserves space for the image in the same axis as the edge against which the button places the image.

var imageColorTransformer: UIConfigurationColorTransformer?

A block that transforms the image color when the button state changes.

var preferredSymbolConfigurationForImage: UIImage.SymbolConfiguration?

A requested configuration object for the button symbol image.

