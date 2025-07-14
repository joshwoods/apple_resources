

- Core Graphics
- CGContext
-  setLineJoin(\_:) 

Instance Method

# setLineJoin(\_:)

Sets the style for the joins of connected lines in a graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setLineJoin(_ join: CGLineJoin)
```

## Parameters 

`join`  

A line join value—CGLineJoin.miter (the default), CGLineJoin.round, or CGLineJoin.bevel. See CGPath.

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

func setLineWidth(CGFloat)

Sets the line width for a graphics context.

func setMiterLimit(CGFloat)

Sets the miter limit for the joins of connected lines in a graphics context.

func setPatternPhase(CGSize)

Sets the pattern phase of a context.

func setFillPattern(CGPattern, colorComponents: UnsafePointer&lt;CGFloat>)

Sets the fill pattern in the specified graphics context.

func setShouldAntialias(Bool)

Sets antialiasing on or off for a graphics context.

