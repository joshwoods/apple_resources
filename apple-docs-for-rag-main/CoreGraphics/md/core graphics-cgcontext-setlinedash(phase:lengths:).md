

- Core Graphics
- CGContext
-  setLineDash(phase:lengths:) 

Instance Method

# setLineDash(phase:lengths:)

Sets the pattern for drawing dashed lines.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setLineDash(
    phase: CGFloat,
    lengths: [CGFloat]
)
```

## Parameters 

`phase`  

A value that specifies how far into the dash pattern the line starts, in units of the user space. For example, a value of `0` draws a line starting with the beginning of a dash pattern, and a value of `3` means the line is drawn with the dash pattern starting at three units from its beginning.

`lengths`  

An array of values that specify the lengths, in user space coordinates, of the painted and unpainted segments of the dash pattern.

For example, the array `[2,3]` sets a dash pattern that alternates between a 2-unit-long painted segment and a 3-unit-long unpainted segment. The array `[1,3,4,2]` sets the pattern to a 1-unit painted segment, a 3-unit unpainted segment, a 4-unit painted segment, and a 2-unit unpainted segment.Pass an empty array to clear the dash pattern so that all stroke drawing in the context uses solid lines.

## See Also

### Setting Path Drawing Options

func setAllowsAntialiasing(Bool)

Sets whether or not to allow antialiasing for a graphics context.

func setFlatness(CGFloat)

Sets the accuracy of curved paths in a graphics context.

func setLineCap(CGLineCap)

Sets the style for the endpoints of lines drawn in a graphics context.

func setLineJoin(CGLineJoin)

Sets the style for the joins of connected lines in a graphics context.

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

