

- AppKit
- NSWindow
- NSWindow.Depth
-  availableDepths 

Type Property

# availableDepths

An array that contains all available windows depths.

macOS 10.9+Swift 4.0+

``` source
static var availableDepths: [NSWindow.Depth] { get }
```

## See Also

### Accessing Depth Details

static func bestDepth(colorSpaceName: NSColorSpaceName, bitsPerSample: Int, bitsPerPixel: Int, isPlanar: Bool) -> (NSWindow.Depth, isExactMatch: Bool)

Determines the best window depth that most closely matches the given properties.

var bitsPerPixel: Int

Returns the bits per pixel for the specified window depth.

var bitsPerSample: Int

Returns the bits per sample for the specified window depth.

var colorSpaceName: NSColorSpaceName?

Returns the name of the color space corresponding to the passed window depth.

var isPlanar: Bool

Returns whether the specified window depth is planar.

