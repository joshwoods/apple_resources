

- Core Text
-  CTGlyphInfo 

Class

# CTGlyphInfo

Override a font’s specified mapping from Unicode to the glyph ID.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CTGlyphInfo
```

## Topics

### Getting the GlyphInfo Type

func CTGlyphInfoGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier of the glyph info object

### Creating GlyphInfo Objects

func CTGlyphInfoCreateWithGlyphName(CFString, CTFont, CFString) -> CTGlyphInfo?

Creates an immutable glyph info object with a glyph name.

func CTGlyphInfoCreateWithGlyph(CGGlyph, CTFont, CFString) -> CTGlyphInfo?

Creates an immutable glyph info object with a glyph index.

func CTGlyphInfoCreateWithCharacterIdentifier(CGFontIndex, CTCharacterCollection, CFString) -> CTGlyphInfo?

Creates an immutable glyph info object with a character identifier.

### Getting GlyphInfo Data

func CTGlyphInfoGetGlyphName(CTGlyphInfo) -> CFString?

Retrieves the glyph name for a glyph info object, if that object exists.

func CTGlyphInfoGetCharacterIdentifier(CTGlyphInfo) -> CGFontIndex

Gets the character identifier for a glyph info object.

func CTGlyphInfoGetCharacterCollection(CTGlyphInfo) -> CTCharacterCollection

Gets the character collection for a glyph info object.

func CTGlyphInfoGetGlyph(CTGlyphInfo) -> CGGlyph

Retrieves the glyph for a glyph info, if that object exists.

### Constants

enum CTCharacterCollection

Constants that specify character collections.

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

class CTTypesetter

A typesetter which performs line layout.

