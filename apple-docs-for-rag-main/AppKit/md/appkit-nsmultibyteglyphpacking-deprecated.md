

- AppKit
-  NSMultibyteGlyphPacking Deprecated

Enumeration

# NSMultibyteGlyphPacking

A constant for glyph packing.

macOS 10.0–10.13Deprecated

``` source
enum NSMultibyteGlyphPacking
```

## Overview

Cocoa stores all text data as Unicode. The text system converts Unicode into glyph IDs and places them in 1-, 2-, or 4-byte storage depending on the context. To render text, you must convert the storage into a format the text engine understands. The following constants describe the glyph packing schemes the text rendering engine can use. They are used to extract glyphs from a font for making a multibyte (or single-byte) array of glyphs for passing to an interpreter, such as the window server, which expects a big-endian multibyte stream (that is, “packed glyphs”) instead of a pure `NSGlyph` stream. They’re used by `glyphPacking`. With Quartz, the engine always expects the format to be in 2-byte short array, so `NSNativeShortGlyphPacking` is the only format currently in use.

## Topics

### Packing Options

case nativeShortGlyphPacking

The native format for macOS.

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

### Enumerations

Glyph Attributes

Attributes that are used only inside the glyph generation machinery, but must also be shared between components.

enum NSOpenGLGlobalOption

Constants that specify OpenGL options.

Deprecated

Data Entry Types

These constants specify how a cell formats numeric data.

Anonymous

Additional Writing Directions

Additional values to be added to NSWritingDirection.leftToRight or NSWritingDirection.rightToLeft, when used with writingDirection.

Return values for modal operations

Historical return values for runModal(for:) and runModalSession(_:).

Tags of Views in the FontPanel

These constants are obsolete and should not be used.

