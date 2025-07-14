

- AppKit
-  NSGlyphGenerator 

Class

# NSGlyphGenerator

An object that performs the initial, nominal glyph generation phase in the layout process.

macOS

``` source
class NSGlyphGenerator
```

## Overview

The nominal glyph generation pass essentially generates one glyph per character; the typesetter may later make substitutions in the glyph stream, for example, changing an acute accent glyph followed by an “e” glyph into a single acute-accented “é” glyph.

NSGlyphGenerator communicates via the NSGlyphStorage protocol. An example of a class that conforms to the protocol is NSLayoutManager.

## Topics

### Obtaining a glyph generator

class var shared: NSGlyphGenerator

Returns a shared instance of `NSGlyphGenerator`.

### Generating glyphs

func generateGlyphs(for: any NSGlyphStorage, desiredNumberOfCharacters: Int, glyphIndex: UnsafeMutablePointer&lt;Int>?, characterIndex: UnsafeMutablePointer&lt;Int>?)

Generates glyphs for the specified glyph storage object (`NSLayoutManager` by default).

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Glyphs

typealias NSGlyph

The type used to specify glyphs.

protocol NSGlyphStorage

A set of methods that a glyph storage object must implement to interact properly with NSGlyphGenerator.

class NSGlyphInfo

A glyph attribute in an attributed string.

Reserved Glyph Codes

These constants define reserved glyph codes.

enum NSFontRenderingMode

The font rendering mode.

