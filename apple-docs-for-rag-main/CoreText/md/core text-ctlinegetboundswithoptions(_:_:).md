

- Core Text
-  CTLineGetBoundsWithOptions(\_:\_:) 

Function

# CTLineGetBoundsWithOptions(\_:\_:)

Calculates the bounds for a line.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineGetBoundsWithOptions(
    _ line: CTLine,
    _ options: CTLineBoundsOptions
) -> CGRect
```

## Parameters 

`line`  

The line for which you calculate the bounds.

`options`  

Desired options or `0` if none.

## Return Value

The bounds of the line as specified by the type and options, such that the coordinate origin is coincident with the line origin and the rect origin is at the bottom left. If the line is invalid, this function will return CGRectNull.

## See Also

### Related Documentation

struct CTLineBoundsOptions

Options for getting the bounds of a line of text.

### Measuring the Glyph Run

func CTRunGetTypographicBounds(CTRun, CFRange, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?) -> Double

Gets the typographic bounds of the run.

func CTRunGetImageBounds(CTRun, CGContext?, CFRange) -> CGRect

Calculates the image bounds for a glyph range.

func CTRunGetBaseAdvancesAndOrigins(CTRun, CFRange, UnsafeMutablePointer&lt;CGSize>?, UnsafeMutablePointer&lt;CGPoint>?)

Copies a range of base advances and origins into user-provided buffers.

