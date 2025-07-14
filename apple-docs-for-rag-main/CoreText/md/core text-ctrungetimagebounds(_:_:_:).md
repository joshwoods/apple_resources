

- Core Text
-  CTRunGetImageBounds(\_:\_:\_:) 

Function

# CTRunGetImageBounds(\_:\_:\_:)

Calculates the image bounds for a glyph range.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunGetImageBounds(
    _ run: CTRun,
    _ context: CGContext?,
    _ range: CFRange
) -> CGRect
```

## Parameters 

`run`  

The run for which to calculate the image bounds.

`context`  

The context for the image bounds being calculated. This is required because the context could have settings in it that would cause changes in the image bounds.

`range`  

The portion of the run to measure. If the length of the range is set to `0`, then the measure operation continues from the start index of the range to the end of the run.

## Return Value

A rectangle that tightly encloses the paths of the run’s glyphs, or, if `run`, `context`, or `range` is invalid, CGRectNull.

## See Also

### Measuring the Glyph Run

func CTLineGetBoundsWithOptions(CTLine, CTLineBoundsOptions) -> CGRect

Calculates the bounds for a line.

func CTRunGetTypographicBounds(CTRun, CFRange, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?) -> Double

Gets the typographic bounds of the run.

func CTRunGetBaseAdvancesAndOrigins(CTRun, CFRange, UnsafeMutablePointer&lt;CGSize>?, UnsafeMutablePointer&lt;CGPoint>?)

Copies a range of base advances and origins into user-provided buffers.

