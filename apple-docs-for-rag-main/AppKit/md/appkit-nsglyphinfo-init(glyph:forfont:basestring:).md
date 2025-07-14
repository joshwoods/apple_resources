

- AppKit
- NSGlyphInfo
-  init(glyph:forFont:baseString:) 

Initializer

# init(glyph:forFont:baseString:)

Instantiates and returns a glyph information object using a glyph index and a specified font.

macOS

``` source
init?(
    glyph: NSGlyph,
    forFont font: NSFont,
    baseString string: String
)
```

``` source
init?(
    glyph: NSGlyph,
    for font: NSFont,
    baseString string: String
)
```

## Parameters 

`glyph`  

The identifier of the glyph.

`font`  

The font object to be associated with the returned `NSGlyphInfo` object,

`string`  

The part of the attributed string the returned instance is intended to override.

## Return Value

The created `NSGlyphInfo` object or `nil` if the object couldn’t be created.

## See Also

### Deprecated

init?(characterIdentifier: Int, collection: NSCharacterCollection, baseString: String)

Instantiates and returns an `NSGlyphInfo` object using a character identifier and a character collection.

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

