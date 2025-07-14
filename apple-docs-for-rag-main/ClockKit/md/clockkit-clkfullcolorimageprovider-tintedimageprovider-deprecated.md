

- ClockKit
- CLKFullColorImageProvider
-  tintedImageProvider Deprecated

Instance Property

# tintedImageProvider

An image provider that produces alternative images for tinted graphic complications.

watchOS 6.0–9.0Deprecated

``` source
var tintedImageProvider: CLKImageProvider? { get set }
```

## Discussion

By default, when the system displays a graphic complication using the tinted mode, it desaturates the full-color image stored in the image property. To provide an alternative template image instead, create an image provider and assign it to the tintedImageProvider property.

Tinted graphic complications interpret the tinted image provider as follows:

- The graphic complication ignores the tintColor property.

- The onePieceImage property returns a single template image. The system sets the image’s color based on the watch-face color the user selected. This property is the only one required to provide tinted images.

- The twoPieceImageForeground and twoPieceImageBackground properties define a two-piece image. Both the foreground and background are template images. The complication layers the foreground image over the background image, and selects the color for both images based on the watch-face color. When applicable, the system displays two-piece images instead of the one-piece images.

## See Also

### Getting the Image Data

var image: UIImage

The full-color image to display.

Deprecated

