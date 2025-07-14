

- Core Text
-  CTRunGetTypographicBounds(\_:\_:\_:\_:\_:) 

Function

# CTRunGetTypographicBounds(\_:\_:\_:\_:\_:)

Gets the typographic bounds of the run.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunGetTypographicBounds(
    _ run: CTRun,
    _ range: CFRange,
    _ ascent: UnsafeMutablePointer?,
    _ descent: UnsafeMutablePointer?,
    _ leading: UnsafeMutablePointer?
) -> Double
```

## Parameters 

`run`  

The run for which to calculate the typographic bounds.

`range`  

The portion of the run to measure. If the length of the range is set to `0`, then the measure operation continues from the range’s start index to the end of the run.

`ascent`  

On output, the ascent of the run. This can be set to `NULL` if not needed.

`descent`  

On output, the descent of the run. This can be set to `NULL` if not needed.

`leading`  

On output, the leading of the run. This can be set to `NULL` if not needed.

## Return Value

The typographic width of the run, or if `run` or `range` is invalid, `0`.

## See Also

### Measuring the Glyph Run

func CTLineGetBoundsWithOptions(CTLine, CTLineBoundsOptions) -> CGRect

Calculates the bounds for a line.

func CTRunGetImageBounds(CTRun, CGContext?, CFRange) -> CGRect

Calculates the image bounds for a glyph range.

func CTRunGetBaseAdvancesAndOrigins(CTRun, CFRange, UnsafeMutablePointer&lt;CGSize>?, UnsafeMutablePointer&lt;CGPoint>?)

Copies a range of base advances and origins into user-provided buffers.

