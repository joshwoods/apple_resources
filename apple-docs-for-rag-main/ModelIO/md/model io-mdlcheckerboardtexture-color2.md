

- Model I/O
- MDLCheckerboardTexture
-  color2 

Instance Property

# color2

The color for the other half of the squares in the checkerboard pattern.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var color2: CGColor? { get set }
```

## Discussion

This color appears in the second square from top left (in either direction) of the generated pattern, and in alternate squares thereafter.

Changing the divisions, color1, or color2 properties invalidates the cache, causing Model I/O to regenerate texel data the next time it is needed.

## See Also

### Configuring the Checkerboard Pattern

var color1: CGColor?

The color for half of the squares in the checkerboard pattern.

var divisions: Float

The number of squares along each dimension in the checkerboard pattern.

