

- Core Text
-  CTRun 

Class

# CTRun

A glyph run.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CTRun
```

## Overview

A glyph run is a set of consecutive glyphs sharing the same attributes and direction.

The typesetter creates glyph runs as it produces lines from character strings, attributes, and font objects. That is, a line is constructed of one or more glyphs runs. Glyph runs can draw themselves into a graphic context, if desired, although most users have no need to interact directly with glyph runs.

## Topics

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

func CTRunGetStringIndices(CTRun, CFRange, UnsafeMutablePointer&lt;CFIndex>)

Copies a range of string indices into a user-provided buffer.

func CTRunGetStringRange(CTRun) -> CFRange

Gets the range of characters that originally spawned the glyphs in the run.

### Measuring the Glyph Run

func CTLineGetBoundsWithOptions(CTLine, CTLineBoundsOptions) -> CGRect

Calculates the bounds for a line.

func CTRunGetTypographicBounds(CTRun, CFRange, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?) -> Double

Gets the typographic bounds of the run.

func CTRunGetImageBounds(CTRun, CGContext?, CFRange) -> CGRect

Calculates the image bounds for a glyph range.

func CTRunGetBaseAdvancesAndOrigins(CTRun, CFRange, UnsafeMutablePointer&lt;CGSize>?, UnsafeMutablePointer&lt;CGPoint>?)

Copies a range of base advances and origins into user-provided buffers.

### Drawing the Glyph Run

func CTRunDraw(CTRun, CGContext, CFRange)

Draws a complete run or part of one.

func CTRunGetTextMatrix(CTRun) -> CGAffineTransform

Returns the text matrix needed to draw this run.

### Getting the Type Identifier

func CTRunGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier of the run object.

### Constants

struct CTRunStatus

A bitfield that represents the disposition of the run.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Opaque Types

class CTFont

A font object.

class CTFontCollection

A font collection.

class CTFontDescriptor

A font descriptor.

class CTFrame

A frame.

class CTFramesetter

Generate text frames.

class CTGlyphInfo

Override a font’s specified mapping from Unicode to the glyph ID.

class CTLine

A line of text.

class CTParagraphStyle

Paragraph or ruler attributes in an attributed string.

class CTRunDelegate

A run delegate.

class CTTextTab

A tab in a paragraph style, storing an alignment type and location.

class CTTypesetter

A typesetter which performs line layout.

