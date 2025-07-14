

- AppKit
- NSWindow
- NSWindow.Depth
-  colorSpaceName 

Instance Property

# colorSpaceName

Returns the name of the color space corresponding to the passed window depth.

macOS

``` source
var colorSpaceName: NSColorSpaceName? { get }
```

## Discussion

Returns the color space name for the specified `depth`. For example, the returned color space name can be calibratedRGB, or deviceCMYK.

## See Also

### Working with Window Depths

var bitsPerPixel: Int

Returns the bits per pixel for the specified window depth.

var bitsPerSample: Int

Returns the bits per sample for the specified window depth.

var numberOfColorComponents: Int

Returns the number of color components in the specified color space.

var isPlanar: Bool

Returns whether the specified window depth is planar.

func canRepresent(NSDisplayGamut) -> Bool

A Boolean value that indicates if the window and its screen use a color space that can represent the specified display gamut.

