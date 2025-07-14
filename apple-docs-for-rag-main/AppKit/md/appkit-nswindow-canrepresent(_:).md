

- AppKit
- NSWindow
-  canRepresent(\_:) 

Instance Method

# canRepresent(\_:)

A Boolean value that indicates if the window and its screen use a color space that can represent the specified display gamut.

macOS 10.12+

``` source
@MainActor
func canRepresent(_ displayGamut: NSDisplayGamut) -> Bool
```

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

var isPlanar: Bool

Returns whether the specified window depth is planar.

