

- Core Graphics
- CGContext
-  strokePath() 

Instance Method

# strokePath()

Paints a line along the current path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func strokePath()
```

## Discussion

The line width and stroke color of the context’s graphics state are used to paint the path. The current path is cleared as a side effect of calling this function.

## See Also

### Drawing the Current Graphics Path

func drawPath(using: CGPathDrawingMode)

Draws the current path using the provided drawing mode.

enum CGPathDrawingMode

Options for rendering a path.

func fillPath(using: CGPathFillRule)

Paints the area within the current path, as determined by the specified fill rule.

