

- AppKit
- NSColorSpaceName
-  numberOfColorComponents 

Instance Property

# numberOfColorComponents

Returns the number of color components in the specified color space.

macOS

``` source
var numberOfColorComponents: Int { get }
```

## Discussion

Returns the number of color components in the color space whose name is provided by `colorSpaceName`.

## See Also

### Working with Window Depths

var bitsPerPixel: Int

Returns the bits per pixel for the specified window depth.

var bitsPerSample: Int

Returns the bits per sample for the specified window depth.

var colorSpaceName: NSColorSpaceName?

Returns the name of the color space corresponding to the passed window depth.

var isPlanar: Bool

Returns whether the specified window depth is planar.

func canRepresent(NSDisplayGamut) -> Bool

A Boolean value that indicates if the window and its screen use a color space that can represent the specified display gamut.

