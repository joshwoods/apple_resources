

- Core Text
-  CTLineGetGlyphRuns(\_:) 

Function

# CTLineGetGlyphRuns(\_:)

Returns the array of glyph runs that make up the line object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineGetGlyphRuns(_ line: CTLine) -> CFArray
```

## Parameters 

`line`  

The line whose glyph run array is returned.

## Return Value

A CFArray containing the CTRun objects that make up the line.

## See Also

### Getting Line Data

func CTLineGetGlyphCount(CTLine) -> CFIndex

Returns the total glyph count for the line object.

func CTLineGetStringRange(CTLine) -> CFRange

Gets the range of characters that originally spawned the glyphs in the line.

func CTLineGetPenOffsetForFlush(CTLine, CGFloat, Double) -> Double

Gets the pen offset required to draw flush text.

