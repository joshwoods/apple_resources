

- Core Text
-  CTRunGetGlyphs(\_:\_:\_:) 

Function

# CTRunGetGlyphs(\_:\_:\_:)

Copies a range of glyphs into a user-provided buffer.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunGetGlyphs(
    _ run: CTRun,
    _ range: CFRange,
    _ buffer: UnsafeMutablePointer
)
```

## Parameters 

`run`  

The run from which to copy glyphs.

`range`  

The range of glyphs to copy. If the length of the range is set to `0`, then the copy operation continues from the range’s start index to the end of the run.

`buffer`  

The buffer the glyphs are copied to. The buffer must be allocated to at least the value specified by the range’s length.

## See Also

### Getting Glyph Run Data

func CTRunGetGlyphCount(CTRun) -> CFIndex

Gets the glyph count for the run.

func CTRunGetAttributes(CTRun) -> CFDictionary

Returns the attribute dictionary that was used to create the glyph run.

func CTRunGetStatus(CTRun) -> CTRunStatus

Returns the run’s status.

func CTRunGetGlyphsPtr(CTRun) -> UnsafePointer&lt;CGGlyph>?

Returns a direct pointer for the glyph array stored in the run.

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

