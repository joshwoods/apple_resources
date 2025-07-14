

- Core Text
-  CTTypesetter 

Class

# CTTypesetter

A typesetter which performs line layout.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CTTypesetter
```

## Overview

Line layout includes word wrapping, hyphenation, and line breaking in either vertical or horizontal rectangles. A typesetter object takes as input an attributed string and produces a line of typeset glyphs (composed into glyph runs) in a CTLine object. The typesetter performs character-to-glyph encoding, glyph ordering, and positional operations, such as kerning, tracking, and baseline adjustments. If multiline layout is needed, it is performed by a CTFramesetter object, which calls into the typesetter to generate the typeset lines to fill the frame.

A CTFramesetter encapsulates a typesetter and provides a reference to it as a convenience, but a caller may also choose to create a freestanding typesetter.

## Topics

### Creating a Typesetter

func CTTypesetterCreateWithAttributedString(CFAttributedString) -> CTTypesetter

Creates an immutable typesetter object using an attributed string.

func CTTypesetterCreateWithAttributedStringAndOptions(CFAttributedString, CFDictionary?) -> CTTypesetter?

Creates an immutable typesetter object using an attributed string and a dictionary of options.

### Creating Lines

func CTTypesetterCreateLine(CTTypesetter, CFRange) -> CTLine

Creates an immutable line from the typesetter.

func CTTypesetterCreateLineWithOffset(CTTypesetter, CFRange, Double) -> CTLine

Creates an immutable line from the typesetter at a specified line offset.

### Breaking Lines

func CTTypesetterSuggestLineBreak(CTTypesetter, CFIndex, Double) -> CFIndex

Suggests a contextual line breakpoint based on the width provided.

func CTTypesetterSuggestLineBreakWithOffset(CTTypesetter, CFIndex, Double, Double) -> CFIndex

Suggests a contextual line breakpoint based on the width provided and the specified offset.

func CTTypesetterSuggestClusterBreak(CTTypesetter, CFIndex, Double) -> CFIndex

Suggests a cluster line breakpoint based on the width provided.

func CTTypesetterSuggestClusterBreakWithOffset(CTTypesetter, CFIndex, Double, Double) -> CFIndex

Suggests a cluster line breakpoint based on the specified width and line offset.

### Getting the Type Identifier

func CTTypesetterGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier of the typesetter object.

### Constants

Typesetter Options

Control aspects of the typesetter’s text processing.

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

class CTRun

A glyph run.

class CTRunDelegate

A run delegate.

class CTTextTab

A tab in a paragraph style, storing an alignment type and location.

