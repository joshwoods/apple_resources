

- Core Text
-  CTRunGetAdvancesPtr(\_:) 

Function

# CTRunGetAdvancesPtr(\_:)

Returns a direct pointer for the glyph advance array stored in the run.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunGetAdvancesPtr(_ run: CTRun) -> UnsafePointer?
```

## Parameters 

`run`  

The run whose advances you wish to access.

## Return Value

A valid pointer to an array of `CGSize` structures representing the glyph advance array or `NULL`.

## Discussion

The advance array will have a length equal to the value returned by CTRunGetGlyphCount(_:). The caller should be prepared for this function to return `NULL` even if there are glyphs in the stream. Should this function return `NULL`, the caller needs allocate its own buffer and call CTRunGetAdvances(_:_:_:) to fetch the advances. Note that advances alone are not sufficient for correctly positioning glyphs in a line, as a run may have a non-identity matrix or the initial glyph in a line may have a non-zero origin; callers should consider using positions instead.

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

func CTRunGetAdvances(CTRun, CFRange, UnsafeMutablePointer&lt;CGSize>)

Copies a range of glyph advances into a user-provided buffer.

func CTRunGetStringIndicesPtr(CTRun) -> UnsafePointer&lt;CFIndex>?

Returns a direct pointer for the string indices stored in the run.

func CTRunGetStringIndices(CTRun, CFRange, UnsafeMutablePointer&lt;CFIndex>)

Copies a range of string indices into a user-provided buffer.

func CTRunGetStringRange(CTRun) -> CFRange

Gets the range of characters that originally spawned the glyphs in the run.

