

- Core Text
-  CTRunGetGlyphCount(\_:) 

Function

# CTRunGetGlyphCount(\_:)

Gets the glyph count for the run.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunGetGlyphCount(_ run: CTRun) -> CFIndex
```

## Parameters 

`run`  

The run for which to return the glyph count.

## Return Value

The number of glyphs that the run contains, or if there are no glyphs in this run, a value of `0`.

## See Also

### Getting Glyph Run Data

func CTRunGetAttributes(CTRun) -> CFDictionary

Returns the attribute dictionary that was used to create the glyph run.

func CTRunGetStatus(CTRun) -> CTRunStatus

Returns the run’s status.

func CTRunGetGlyphsPtr(CTRun) -> UnsafePointer&lt;CGGlyph>?

Returns a direct pointer for the glyph array stored in the run.

func CTRunGetGlyphs(CTRun, CFRange, UnsafeMutablePointer&lt;CGGlyph>)

Copies a range of glyphs into a user-provided buffer.

func CTRunGetPositionsPtr(CTRun) -> UnsafePointer&lt;CGPoint>?

Returns a direct pointer for the glyph position array stored in the run.

func CTRunGetPositions(CTRun, CFRange, UnsafeMutablePointer&lt;CGPoint>)

Copies a range of glyph positions into a user-provided buffer.

func CTRunGetAdvancesPtr(CTRun) -> UnsafePointer&lt;CGSize>?

Returns a direct pointer for the glyph advance array stored in the run.

func CTRunGetAdvances(CTRun, CFRange, UnsafeMutablePointer&lt;CGSize>)

Copies a range of glyph advances into a user-provided buffer.

func CTRunGetStringIndicesPtr(CTRun) -> UnsafePointer&lt;CFIndex>?

Returns a direct pointer for the string indices stored in the run.

func CTRunGetStringIndices(CTRun, CFRange, UnsafeMutablePointer&lt;CFIndex>)

Copies a range of string indices into a user-provided buffer.

func CTRunGetStringRange(CTRun) -> CFRange

Gets the range of characters that originally spawned the glyphs in the run.

