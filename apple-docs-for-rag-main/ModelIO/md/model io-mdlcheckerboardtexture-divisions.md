

- Model I/O
- MDLCheckerboardTexture
-  divisions 

Instance Property

# divisions

The number of squares along each dimension in the checkerboard pattern.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var divisions: Float { get set }
```

## Discussion

For example, a value of 2 creates a checkerboard pattern of four squares (a 2 x 2 grid), where the top-left and bottom-right squares use the color1 color and the other two squares use the color2 color. A value of 4 creates a pattern of 16 squares (a 4 x 4 grid), and so on.

Changing the divisions, color1, or color2 properties invalidates the cache, causing Model I/O to regenerate texel data the next time it is needed.

## See Also

### Configuring the Checkerboard Pattern

var color1: CGColor?

The color for half of the squares in the checkerboard pattern.

var color2: CGColor?

The color for the other half of the squares in the checkerboard pattern.

