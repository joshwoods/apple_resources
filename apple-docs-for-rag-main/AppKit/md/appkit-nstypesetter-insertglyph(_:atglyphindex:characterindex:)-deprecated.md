

- AppKit
- NSTypesetter
-  insertGlyph(\_:atGlyphIndex:characterIndex:) Deprecated

Instance Method

# insertGlyph(\_:atGlyphIndex:characterIndex:)

Enables the typesetter to insert a new glyph into the stream.

macOS 10.3–10.13Deprecated

``` source
func insertGlyph(
    _ glyph: NSGlyph,
    atGlyphIndex glyphIndex: Int,
    characterIndex: Int
)
```

## Parameters 

`glyph`  

The glyph to insert into the glyph cache.

`glyphIndex`  

The index at which to insert `glyph`.

`characterIndex`  

The index of the character that `glyph` maps to. If the glyph is mapped to several characters, `charIndex` should indicate the first character to which it’s mapped.

## Discussion

The standard typesetter uses this method for inserting hyphenation glyphs. Because this method keeps the glyph caches synchronized, subclasses should always use this method to insert glyphs instead of calling layoutManager directly.

A subclass can override this method to interact with custom glyph storage.

## See Also

### Deprecated

func actionForControlCharacter(at: Int) -> NSTypesetterControlCharacterAction

Returns the action associated with a control character.

func deleteGlyphs(in: NSRange)

Deletes the specified glyphs from the glyph cache maintained by the layout manager.

Deprecated

func substituteGlyphs(in: NSRange, withGlyphs: UnsafeMutablePointer&lt;NSGlyph>!)

Replaces the specified glyphs with specified replacement glyphs.

Deprecated

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;NSGlyph>!, characterIndexes: UnsafeMutablePointer&lt;Int>!, glyphInscriptions: UnsafeMutablePointer&lt;NSGlyphInscription>!, elasticBits: UnsafeMutablePointer&lt;ObjCBool>!, bidiLevels: UnsafeMutablePointer&lt;UInt8>!) -> Int

Extracts the information needed to lay out the provided glyphs from the provided range.

Deprecated

struct NSTypesetterControlCharacterAction

The following constants are possible values returned by the actionForControlCharacter(at:) method to determine the action associated with a control character.

