

- Core Text
-  CTLine 

Class

# CTLine

A line of text.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CTLine
```

## Overview

A `CTLine` object contains an array of glyph runs. Line objects are created by the typesetter during a framesetting operation and can draw themselves directly into a graphics context.

## Topics

### Creating Lines

func CTLineCreateWithAttributedString(CFAttributedString) -> CTLine

Creates a single immutable line object from an attributed string.

func CTLineCreateTruncatedLine(CTLine, Double, CTLineTruncationType, CTLine?) -> CTLine?

Creates a truncated line from an existing line.

func CTLineCreateJustifiedLine(CTLine, CGFloat, Double) -> CTLine?

Creates a justified line from an existing line.

### Drawing the Line

func CTLineDraw(CTLine, CGContext)

Draws a complete line.

### Getting Line Data

func CTLineGetGlyphCount(CTLine) -> CFIndex

Returns the total glyph count for the line object.

func CTLineGetGlyphRuns(CTLine) -> CFArray

Returns the array of glyph runs that make up the line object.

func CTLineGetStringRange(CTLine) -> CFRange

Gets the range of characters that originally spawned the glyphs in the line.

func CTLineGetPenOffsetForFlush(CTLine, CGFloat, Double) -> Double

Gets the pen offset required to draw flush text.

### Measuring Lines

func CTLineGetImageBounds(CTLine, CGContext?) -> CGRect

Calculates the image bounds for a line.

func CTLineGetTypographicBounds(CTLine, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?, UnsafeMutablePointer&lt;CGFloat>?) -> Double

Calculates the typographic bounds of a line.

func CTLineGetTrailingWhitespaceWidth(CTLine) -> Double

Returns the trailing whitespace width for a line.

### Getting Line Positioning

func CTLineGetStringIndexForPosition(CTLine, CGPoint) -> CFIndex

Performs hit testing.

func CTLineGetOffsetForStringIndex(CTLine, CFIndex, UnsafeMutablePointer&lt;CGFloat>?) -> CGFloat

Determines the graphical offset or offsets for a string index.

func CTLineEnumerateCaretOffsets(CTLine, (Double, CFIndex, Bool, UnsafeMutablePointer&lt;Bool>) -> Void)

Enumerates caret offsets for characters in a line.

### Getting the Type Identifier

func CTLineGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier of the line object.

### Constants

enum CTLineTruncationType

Truncation types required by the CTLineCreateTruncatedLine(_:_:_:_:) function to tell the truncation engine which type of truncation is being requested.

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

class CTParagraphStyle

Paragraph or ruler attributes in an attributed string.

class CTRun

A glyph run.

class CTRunDelegate

A run delegate.

class CTTextTab

A tab in a paragraph style, storing an alignment type and location.

class CTTypesetter

A typesetter which performs line layout.

