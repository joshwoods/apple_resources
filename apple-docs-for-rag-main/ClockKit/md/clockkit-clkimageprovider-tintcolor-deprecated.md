

- ClockKit
- CLKImageProvider
-  tintColor Deprecated

Instance Property

# tintColor

The tint color to apply to the image in a multicolor clock face.

watchOS 2.0–9.0Deprecated

``` source
var tintColor: UIColor? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

For multicolor clock faces, the image provider applies the color in this property to the underlying image. For one-piece images, the color is applied directly to the image. For two-piece images, the color is applied only to the background image.

Specify `nil` to tint the image using the color of the complication template object. If the template doesn’t specify a color, the default color (white) is used.

## See Also

### Getting the Image Data

var onePieceImage: UIImage

The template image to use as a one-piece image.

Deprecated

var twoPieceImageBackground: UIImage?

The background image in a two-piece image.

Deprecated

var twoPieceImageForeground: UIImage?

The foreground image in a two-piece image.

Deprecated

