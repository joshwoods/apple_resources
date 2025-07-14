

- AppKit
- NSWindow
- NSWindow.Depth
-  bitsPerSample 

Instance Property

# bitsPerSample

Returns the bits per sample for the specified window depth.

macOS

``` source
var bitsPerSample: Int { get }
```

## Discussion

Returns the number of bits per sample (bits per pixel in each color component) for the window depth specified by `depth`.

## See Also

### Working with Window Depths

var bitsPerPixel: Int

Returns the bits per pixel for the specified window depth.

var colorSpaceName: NSColorSpaceName?

Returns the name of the color space corresponding to the passed window depth.

var numberOfColorComponents: Int

Returns the number of color components in the specified color space.

var isPlanar: Bool

Returns whether the specified window depth is planar.

func canRepresent(NSDisplayGamut) -> Bool

A Boolean value that indicates if the window and its screen use a color space that can represent the specified display gamut.

