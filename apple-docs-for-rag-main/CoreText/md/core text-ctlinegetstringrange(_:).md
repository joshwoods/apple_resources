

- Core Text
-  CTLineGetStringRange(\_:) 

Function

# CTLineGetStringRange(\_:)

Gets the range of characters that originally spawned the glyphs in the line.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTLineGetStringRange(_ line: CTLine) -> CFRange
```

## Parameters 

`line`  

The line from which to obtain the string range.

## Return Value

A CFRange structure that contains the range over the backing store string that spawned the glyphs, or if the function fails for any reason, an empty range.

## See Also

### Getting Line Data

func CTLineGetGlyphCount(CTLine) -> CFIndex

Returns the total glyph count for the line object.

func CTLineGetGlyphRuns(CTLine) -> CFArray

Returns the array of glyph runs that make up the line object.

func CTLineGetPenOffsetForFlush(CTLine, CGFloat, Double) -> Double

Gets the pen offset required to draw flush text.

