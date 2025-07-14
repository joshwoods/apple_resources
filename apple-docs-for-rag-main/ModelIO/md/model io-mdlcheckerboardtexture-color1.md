

- Model I/O
- MDLCheckerboardTexture
-  color1 

Instance Property

# color1

The color for half of the squares in the checkerboard pattern.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var color1: CGColor? { get set }
```

## Discussion

This color appears in the top left square of the generated pattern, and in alternate squares thereafter.

Changing the divisions, color1, or color2 properties invalidates the cache, causing Model I/O to regenerate texel data the next time it is needed.

## See Also

### Configuring the Checkerboard Pattern

var color2: CGColor?

The color for the other half of the squares in the checkerboard pattern.

var divisions: Float

The number of squares along each dimension in the checkerboard pattern.

