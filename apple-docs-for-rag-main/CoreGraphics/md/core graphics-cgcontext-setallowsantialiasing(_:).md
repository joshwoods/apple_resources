

- Core Graphics
- CGContext
-  setAllowsAntialiasing(\_:) 

Instance Method

# setAllowsAntialiasing(\_:)

Sets whether or not to allow antialiasing for a graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setAllowsAntialiasing(_ allowsAntialiasing: Bool)
```

## Parameters 

`allowsAntialiasing`  

A Boolean value that specifies whether or not to allow antialiasing. Pass `true` to allow antialiasing; `false` otherwise. This parameter is not part of the graphics state.

## Discussion

Core Graphics performs antialiasing for a graphics context if both the `allowsAntialiasing` parameter and the graphics state parameter `shouldAntialias` are `true`.

This parameter is not part of the graphics state.

## See Also

### Setting Path Drawing Options

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

func setMiterLimit(CGFloat)

Sets the miter limit for the joins of connected lines in a graphics context.

func setPatternPhase(CGSize)

Sets the pattern phase of a context.

func setFillPattern(CGPattern, colorComponents: UnsafePointer&lt;CGFloat>)

Sets the fill pattern in the specified graphics context.

func setShouldAntialias(Bool)

Sets antialiasing on or off for a graphics context.

