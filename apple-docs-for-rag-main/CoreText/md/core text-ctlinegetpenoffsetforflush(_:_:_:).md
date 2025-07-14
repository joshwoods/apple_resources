

- Core Text
-  CTLineGetPenOffsetForFlush(\_:\_:\_:) 

Function

# CTLineGetPenOffsetForFlush(\_:\_:\_:)

Gets the pen offset required to draw flush text.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineGetPenOffsetForFlush(
    _ line: CTLine,
    _ flushFactor: CGFloat,
    _ flushWidth: Double
) -> Double
```

## Parameters 

`line`  

The line from which to obtain a flush position.

`flushFactor`  

Determines the type of flushness. A `flushFactor` of `0` or less indicates left flush. A `flushFactor` of `1.0` or more indicates right flush. Flush factors between `0` and `1.0` indicate varying degrees of center flush, with a value of `0.5` being totally center flush.

`flushWidth`  

Specifies the width to which the flushness operation should apply.

## Return Value

The offset from the current pen position for the flush operation.

## See Also

### Getting Line Data

func CTLineGetGlyphCount(CTLine) -> CFIndex

Returns the total glyph count for the line object.

func CTLineGetGlyphRuns(CTLine) -> CFArray

Returns the array of glyph runs that make up the line object.

func CTLineGetStringRange(CTLine) -> CFRange

Gets the range of characters that originally spawned the glyphs in the line.

