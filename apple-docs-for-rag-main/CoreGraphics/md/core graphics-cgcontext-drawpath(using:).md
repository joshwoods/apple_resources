

- Core Graphics
- CGContext
-  drawPath(using:) 

Instance Method

# drawPath(using:)

Draws the current path using the provided drawing mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func drawPath(using mode: CGPathDrawingMode)
```

## Parameters 

`mode`  

A path drawing mode constant—CGPathDrawingMode.fill, CGPathDrawingMode.eoFill, CGPathDrawingMode.stroke, CGPathDrawingMode.fillStroke, or CGPathDrawingMode.eoFillStroke. For a discussion of these constants, see CGPath.

## Discussion

The current path is cleared as a side effect of calling this function.

## See Also

### Drawing the Current Graphics Path

enum CGPathDrawingMode

Options for rendering a path.

func fillPath(using: CGPathFillRule)

Paints the area within the current path, as determined by the specified fill rule.

func strokePath()

Paints a line along the current path.

