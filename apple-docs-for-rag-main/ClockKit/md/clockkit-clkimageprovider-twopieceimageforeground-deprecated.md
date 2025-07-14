

- ClockKit
- CLKImageProvider
-  twoPieceImageForeground Deprecated

Instance Property

# twoPieceImageForeground

The foreground image in a two-piece image.

watchOS 2.0–9.0Deprecated

``` source
var twoPieceImageForeground: UIImage? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

The image you specified is tinted white and composited on top of the background image. This image is used only in multicolor environments. You may specify `nil` for this image if you want to display only the background image, but in that case it’s better to use a one-piece image instead.

The image you specify for this property must be a template image—that is, an image where you convey the desired shape using only the alpha channel of the image. The color channels of the image are ignored. Fully and partially opaque areas of the template image are tinted using the appropriate tint color, which is determined by the clock face.

The image provider scales your image as needed to fit the target template. For information about the image sizes to use in different templates, see Apple Watch Human Interface Guidelines.

## See Also

### Related Documentation

convenience init(onePieceImage: UIImage, twoPieceImageBackground: UIImage?, twoPieceImageForeground: UIImage?)

Creates and returns an image provider with both one-piece and two-piece images.

Deprecated

### Getting the Image Data

var onePieceImage: UIImage

The template image to use as a one-piece image.

Deprecated

var tintColor: UIColor?

The tint color to apply to the image in a multicolor clock face.

Deprecated

var twoPieceImageBackground: UIImage?

The background image in a two-piece image.

Deprecated

