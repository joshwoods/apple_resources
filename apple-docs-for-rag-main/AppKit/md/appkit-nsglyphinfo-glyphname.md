

- AppKit
- NSGlyphInfo
-  glyphName 

Instance Property

# glyphName

The receiver’s glyph name.

macOS

``` source
var glyphName: String? { get }
```

## See Also

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

enum NSCharacterCollection

Values that map character identifiers to glyphs.

