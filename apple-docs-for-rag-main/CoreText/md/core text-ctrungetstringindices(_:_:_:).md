

- Core Text
-  CTRunGetStringIndices(\_:\_:\_:) 

Function

# CTRunGetStringIndices(\_:\_:\_:)

Copies a range of string indices into a user-provided buffer.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunGetStringIndices(
    _ run: CTRun,
    _ range: CFRange,
    _ buffer: UnsafeMutablePointer
)
```

## Parameters 

`run`  

The run from which to copy the string indices.

`range`  

The range of string indices to copy. If the length of the range is set to `0`, then the copy operation continues from the range’s start index to the end of the run.

`buffer`  

The buffer to which the string indices are copied. The buffer must be allocated to at least the value specified by the range’s length.

## Discussion

The indices are the character indices that originally spawned the glyphs that make up the run. They can be used to map the glyphs in the run back to the characters in the backing store.

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

func CTRunGetStringRange(CTRun) -> CFRange

Gets the range of characters that originally spawned the glyphs in the run.

