

- AppKit
- NSWindow
- NSWindow.Depth
-  bestDepth(colorSpaceName:bitsPerSample:bitsPerPixel:isPlanar:) 

Type Method

# bestDepth(colorSpaceName:bitsPerSample:bitsPerPixel:isPlanar:)

Determines the best window depth that most closely matches the given properties.

macOS 10.9+Swift 4.0+

``` source
static func bestDepth(
    colorSpaceName: NSColorSpaceName,
    bitsPerSample: Int,
    bitsPerPixel: Int,
    isPlanar: Bool
) -> (NSWindow.Depth, isExactMatch: Bool)
```

## Parameters 

`colorSpaceName`  

The name of a color space to match.

`bitsPerSample`  

The bits per sample to match.

`bitsPerPixel`  

The bits per pixel to match.

`isPlanar`  

A Boolean that indicates whether the window depth is planar.

## Return Value

The window depth that most closely matches the properties this function requests.

## See Also

### Accessing Depth Details

static var availableDepths: [NSWindow.Depth]

An array that contains all available windows depths.

var bitsPerPixel: Int

Returns the bits per pixel for the specified window depth.

var bitsPerSample: Int

Returns the bits per sample for the specified window depth.

var colorSpaceName: NSColorSpaceName?

Returns the name of the color space corresponding to the passed window depth.

var isPlanar: Bool

Returns whether the specified window depth is planar.

