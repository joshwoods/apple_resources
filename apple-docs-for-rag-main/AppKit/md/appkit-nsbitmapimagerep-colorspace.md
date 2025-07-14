

- AppKit
- NSBitmapImageRep
-  colorSpace 

Instance Property

# colorSpace

The color space of the bitmap.

macOS 10.6+

``` source
var colorSpace: NSColorSpace { get }
```

## See Also

### Managing Color Spaces

func converting(to: NSColorSpace, renderingIntent: NSColorRenderingIntent) -> NSBitmapImageRep?

Converts the bitmap image representation to the specified color space.

func retagging(with: NSColorSpace) -> NSBitmapImageRep?

Changes the color space tag of the bitmap image representation.

