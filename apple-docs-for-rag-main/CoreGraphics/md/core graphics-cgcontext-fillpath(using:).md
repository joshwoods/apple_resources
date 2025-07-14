

- Core Graphics
- CGContext
-  fillPath(using:) 

Instance Method

# fillPath(using:)

Paints the area within the current path, as determined by the specified fill rule.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func fillPath(using rule: CGPathFillRule = .winding)
```

## Parameters 

`rule`  

The rule for determining which areas to treat as the interior of the path. See CGPathFillRule.

This parameter defaults to the CGPathFillRule.winding rule if unspecified.

## Discussion

If the current path contains any non-closed subpaths, this method treats each subpath as if it had been closed with the closePath() method, then applies the specified rule to determine which areas to fill.

After filling the path, this method clears the context’s current path.

## See Also

### Drawing the Current Graphics Path

func drawPath(using: CGPathDrawingMode)

Draws the current path using the provided drawing mode.

enum CGPathDrawingMode

Options for rendering a path.

func strokePath()

Paints a line along the current path.

