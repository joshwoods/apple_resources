

- Core Text
-  CTLineGetGlyphCount(\_:) 

Function

# CTLineGetGlyphCount(\_:)

Returns the total glyph count for the line object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineGetGlyphCount(_ line: CTLine) -> CFIndex
```

## Parameters 

`line`  

The line whose glyph count is returned.

## Return Value

The total glyph count for the line passed in.

## Discussion

The total glyph count is equal to the sum of all of the glyphs in the glyph runs forming the line.

## See Also

### Getting Line Data

func CTLineGetGlyphRuns(CTLine) -> CFArray

Returns the array of glyph runs that make up the line object.

func CTLineGetStringRange(CTLine) -> CFRange

Gets the range of characters that originally spawned the glyphs in the line.

func CTLineGetPenOffsetForFlush(CTLine, CGFloat, Double) -> Double

Gets the pen offset required to draw flush text.

