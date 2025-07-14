

- Core Graphics
- CGContext
-  setMiterLimit(\_:) 

Instance Method

# setMiterLimit(\_:)

Sets the miter limit for the joins of connected lines in a graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setMiterLimit(_ limit: CGFloat)
```

## Parameters 

`limit`  

The miter limit to use.

## Discussion

If the current line join style is set to CGLineJoin.miter, the miter limit determines whether the lines should be joined with a bevel instead of a miter. The length of the miter is divided by the line width. If the result is greater than the miter limit, the style is converted to a bevel.

## See Also

### Setting Path Drawing Options

func setAllowsAntialiasing(Bool)

Sets whether or not to allow antialiasing for a graphics context.

func setFlatness(CGFloat)

Sets the accuracy of curved paths in a graphics context.

func setLineCap(CGLineCap)

Sets the style for the endpoints of lines drawn in a graphics context.

func setLineDash(phase: CGFloat, lengths: [CGFloat])

Sets the pattern for drawing dashed lines.

func setLineJoin(CGLineJoin)

Sets the style for the joins of connected lines in a graphics context.

func setLineWidth(CGFloat)

Sets the line width for a graphics context.

func setPatternPhase(CGSize)

Sets the pattern phase of a context.

func setFillPattern(CGPattern, colorComponents: UnsafePointer&lt;CGFloat>)

Sets the fill pattern in the specified graphics context.

func setShouldAntialias(Bool)

Sets antialiasing on or off for a graphics context.

