

- AppKit
-  NSGlyphInfo 

Class

# NSGlyphInfo

A glyph attribute in an attributed string.

macOS

``` source
class NSGlyphInfo
```

## Overview

Glyphs are the graphic representations of characters, stored in a font, that the text system draws on a display or printed page. Before text can be laid out, the layout manager (\NSLayoutManager) generates a stream of glyphs, using the character and font information specified by the attributed string and contained in the font file. NSGlyphInfo represents a glyph attribute value (NSGlyphInfoAttributeName) in an attributed string (NSAttributedString) and provides a means to override the standard glyph generation process and substitute a specified glyph over the attribute’s range.

Glyph attributes are integer values that the layout manager uses to denote special handling for particular glyphs during rendering. NSGlyphInfo enables you to override a font’s built-in mapping from a Unicode character code to a corresponding glyph ID. Overriding the mapping allows you to specify a variant glyph for a given character if the font contains multiple variations for that character or to specify a glyph that doesn’t have a standard mapping (such as some ligature glyphs).

## Topics

### Creating a glyph info object

init?(cgGlyph: CGGlyph, for: NSFont, baseString: String)

Creates a glyph info object from the specified glyph identifier and font informaton.

### Getting information about a glyph info object

var baseString: String

The string containing the character represented by the glyph.

var glyphID: CGGlyph

The glyph identifier, specified as the index into the internal glyph table of the font.

### Deprecated

init?(characterIdentifier: Int, collection: NSCharacterCollection, baseString: String)

Instantiates and returns an `NSGlyphInfo` object using a character identifier and a character collection.

init?(glyph: NSGlyph, forFont: NSFont, baseString: String)

Instantiates and returns a glyph information object using a glyph index and a specified font.

init?(glyphName: String, forFont: NSFont, baseString: String)

Instantiates and returns a glyph information object using a glyph name and a specified font.

var characterIdentifier: Int

The receiver’s character identifier (CID).

var characterCollection: NSCharacterCollection

A value specifying the glyph–to–character identifier mapping of the receiver.

var glyphName: String?

The receiver’s glyph name.

enum NSCharacterCollection

Values that map character identifiers to glyphs.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Glyphs

typealias NSGlyph

The type used to specify glyphs.

protocol NSGlyphStorage

A set of methods that a glyph storage object must implement to interact properly with NSGlyphGenerator.

class NSGlyphGenerator

An object that performs the initial, nominal glyph generation phase in the layout process.

Reserved Glyph Codes

These constants define reserved glyph codes.

enum NSFontRenderingMode

The font rendering mode.

