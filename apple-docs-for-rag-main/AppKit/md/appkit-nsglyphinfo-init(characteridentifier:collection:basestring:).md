

- AppKit
- NSGlyphInfo
-  init(characterIdentifier:collection:baseString:) 

Initializer

# init(characterIdentifier:collection:baseString:)

Instantiates and returns an `NSGlyphInfo` object using a character identifier and a character collection.

macOS

``` source
init?(
    characterIdentifier cid: Int,
    collection characterCollection: NSCharacterCollection,
    baseString string: String
)
```

## Parameters 

`cid`  

A character identifier.

`characterCollection`  

A string constant representing a character collection. Possible values are described in NSCharacterCollection.

`string`  

The part of the attributed string the returned instance is intended to override.

## Return Value

The created `NSGlyphInfo` object or `nil` if the object couldn’t be created.

## See Also

### Related Documentation

Cocoa Text Architecture Guide

### Deprecated

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

