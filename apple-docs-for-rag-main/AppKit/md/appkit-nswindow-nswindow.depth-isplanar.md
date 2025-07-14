

- AppKit
- NSWindow
- NSWindow.Depth
-  isPlanar 

Instance Property

# isPlanar

Returns whether the specified window depth is planar.

macOS

``` source
var isPlanar: Bool { get }
```

## Discussion

Returns true if the specified window `depth` is planar and false if it is not.

## See Also

### Working with Window Depths

var bitsPerPixel: Int

Returns the bits per pixel for the specified window depth.

var bitsPerSample: Int

Returns the bits per sample for the specified window depth.

var colorSpaceName: NSColorSpaceName?

Returns the name of the color space corresponding to the passed window depth.

var numberOfColorComponents: Int

Returns the number of color components in the specified color space.

func canRepresent(NSDisplayGamut) -> Bool

A Boolean value that indicates if the window and its screen use a color space that can represent the specified display gamut.

