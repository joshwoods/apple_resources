

- AppKit
-  NSCharacterCollection 

Enumeration

# NSCharacterCollection

Values that map character identifiers to glyphs.

macOS

``` source
enum NSCharacterCollection
```

## Topics

### Collections

case identityMappingCharacterCollection

Indicates that the character identifier is equal to the glyph index.

case adobeCNS1CharacterCollection

Indicates the Adobe-CNS1 mapping.

case adobeGB1CharacterCollection

Indicates the Adobe-GB1 mapping.

case adobeJapan1CharacterCollection

Indicates the Adobe-Japan1 mapping.

case adobeJapan2CharacterCollection

Indicates the Adobe-Japan2 mapping.

case adobeKorea1CharacterCollection

Indicates the Adobe-Korea1 mapping.

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

