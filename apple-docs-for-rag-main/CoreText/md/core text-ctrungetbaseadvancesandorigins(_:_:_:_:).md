

- Core Text
-  CTRunGetBaseAdvancesAndOrigins(\_:\_:\_:\_:) 

Function

# CTRunGetBaseAdvancesAndOrigins(\_:\_:\_:\_:)

Copies a range of base advances and origins into user-provided buffers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunGetBaseAdvancesAndOrigins(
    _ runRef: CTRun,
    _ range: CFRange,
    _ advancesBuffer: UnsafeMutablePointer?,
    _ originsBuffer: UnsafeMutablePointer?
)
```

## Parameters 

`runRef`  

The run that contains the base advances and origins you wish to copy.

`range`  

The range of values to be copied. If the length of the range is set to `0`, the copy operation continues from the range’s start index to the end of the run.

`advancesBuffer`  

The buffer to which the base advances will be copied, or `NULL`. If not `NULL`, the buffer must allow for at least as many elements as specified by the range’s length.

`originsBuffer`  

The buffer to which the origins will be copied, or `NULL`. If not `NULL`, the buffer must allow for at least as many elements as specified by the range’s length.

## Discussion

A run’s base advances and origins determine the positions of its glyphs but require additional processing before being used for drawing.

Similar to the advances returned by CTRunGetAdvances(_:_:_:), base advances are the displacement from the origin of a glyph to the origin of the next glyph, except base advances do not include any positioning the font layout tables may have done relative to another glyph (such as a mark relative to its base).

The displacement of the current glyph’s origin from the starting position determines the glyph’s actual position, and the displacement of the current glyph’s base advance from the starting position determines the position of the next glyph.

## See Also

### Related Documentation

func CTRunGetAdvances(CTRun, CFRange, UnsafeMutablePointer&lt;CGSize>)

Copies a range of glyph advances into a user-provided buffer.

### Measuring the Glyph Run

func CTLineGetBoundsWithOptions(CTLine, CTLineBoundsOptions) -> CGRect

Calculates the bounds for a line.

func CTRunGetTypographicBounds(CTRun, CFRange, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?) -> Double

Gets the typographic bounds of the run.

func CTRunGetImageBounds(CTRun, CGContext?, CFRange) -> CGRect

Calculates the image bounds for a glyph range.

