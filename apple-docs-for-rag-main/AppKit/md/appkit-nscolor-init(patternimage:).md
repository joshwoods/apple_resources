

- AppKit
- NSColor
-  init(patternImage:) 

Initializer

# init(patternImage:)

Creates a color object that uses the specified image pattern to paint the target area.

macOS

``` source
init(patternImage image: NSImage)
```

## Parameters 

`image`  

The image to use as the pattern for the color object. The image is tiled starting at the bottom of the window. The image is not scaled.

## Return Value

The `NSColor` object. This color object is autoreleased.

## See Also

### Creating a Pattern-Based Color

var patternImage: NSImage

The pattern image used to paint the target area.

