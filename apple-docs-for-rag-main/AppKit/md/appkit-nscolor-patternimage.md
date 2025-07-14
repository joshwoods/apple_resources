

- AppKit
- NSColor
-  patternImage 

Instance Property

# patternImage

The pattern image used to paint the target area.

macOS

``` source
@NSCopying
var patternImage: NSImage { get }
```

## Discussion

This property contains the image (instead of the solid color) to use during drawing. Pattern images are tiled as needed to fill the rendered area.

Do not access this property unless you created the color object using a pattern image. Accessing this property for colors created using other types of color information raises an exception.

## See Also

### Creating a Pattern-Based Color

init(patternImage: NSImage)

Creates a color object that uses the specified image pattern to paint the target area.

