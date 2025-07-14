

- AppKit
- NSGraphicsContext
-  colorRenderingIntent 

Instance Property

# colorRenderingIntent

The color rendering intent in the graphics context’s graphics state.

macOS 10.5+

``` source
var colorRenderingIntent: NSColorRenderingIntent { get set }
```

## Discussion

A value that specifies the rendering intent currently used by the graphics context. For possible values, see NSColorRenderingIntent. The rendering intent specifies how Cocoa should handle colors that are not located within the gamut of the destination color space of a graphics context. If you do not explicitly set the rendering intent, and sampled images are being drawn, NSGraphicsContext uses perceptual rendering intent. Otherwise, NSGraphicsContext uses relative colorimetric rendering intent.

## See Also

### Managing Color Rendering

enum NSColorRenderingIntent

Constants that specify how Cocoa should handle colors that are not located within the destination color space of a graphics context.

