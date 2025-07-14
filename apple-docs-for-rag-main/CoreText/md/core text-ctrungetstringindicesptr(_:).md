

- Core Text
-  CTRunGetStringIndicesPtr(\_:) 

Function

# CTRunGetStringIndicesPtr(\_:)

Returns a direct pointer for the string indices stored in the run.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunGetStringIndicesPtr(_ run: CTRun) -> UnsafePointer?
```

## Parameters 

`run`  

The run for which to return string indices.

## Return Value

A valid pointer to an array of CFIndex structures, or `NULL`.

## Discussion

The indices are the character indices that originally spawned the glyphs that make up the run. They can be used to map the glyphs in the run back to the characters in the backing store. The string indices array will have a length equal to the value returned by CTRunGetGlyphCount(_:). The caller should be prepared for this function to return `NULL` even if there are glyphs in the stream. If this function returns `NULL`, the caller must allocate its own buffer and call CTRunGetStringIndices(_:_:_:) to fetch the indices.

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

func CTRunGetStringIndices(CTRun, CFRange, UnsafeMutablePointer&lt;CFIndex>)

Copies a range of string indices into a user-provided buffer.

func CTRunGetStringRange(CTRun) -> CFRange

Gets the range of characters that originally spawned the glyphs in the run.

