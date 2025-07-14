

- AppKit
-  NSFontRenderingMode 

Enumeration

# NSFontRenderingMode

The font rendering mode.

macOS

``` source
enum NSFontRenderingMode
```

## Topics

### Constants

case defaultRenderingMode

Determines the actual mode based on the user preference settings.

case antialiasedRenderingMode

Specifies antialiased, floating-point advancements rendering mode (synonymous with printerFont).

case integerAdvancementsRenderingMode

Specifies integer advancements rendering mode.

case antialiasedIntegerAdvancementsRenderingMode

Specifies antialiased, integer advancements rendering mode.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Glyphs

typealias NSGlyph

The type used to specify glyphs.

protocol NSGlyphStorage

A set of methods that a glyph storage object must implement to interact properly with NSGlyphGenerator.

class NSGlyphGenerator

An object that performs the initial, nominal glyph generation phase in the layout process.

class NSGlyphInfo

A glyph attribute in an attributed string.

Reserved Glyph Codes

These constants define reserved glyph codes.

