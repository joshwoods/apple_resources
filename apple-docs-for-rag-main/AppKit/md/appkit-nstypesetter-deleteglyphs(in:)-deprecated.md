

- AppKit
- NSTypesetter
-  deleteGlyphs(in:) Deprecated

Instance Method

# deleteGlyphs(in:)

Deletes the specified glyphs from the glyph cache maintained by the layout manager.

macOS 10.3–10.13Deprecated

``` source
func deleteGlyphs(in glyphRange: NSRange)
```

## Parameters 

`glyphRange`  

The range of glyphs to be deleted.

## Discussion

A subclass can override this method to interact with custom glyph storage.

## See Also

### Deprecated

func actionForControlCharacter(at: Int) -> NSTypesetterControlCharacterAction

Returns the action associated with a control character.

func substituteGlyphs(in: NSRange, withGlyphs: UnsafeMutablePointer&lt;NSGlyph>!)

Replaces the specified glyphs with specified replacement glyphs.

Deprecated

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;NSGlyph>!, characterIndexes: UnsafeMutablePointer&lt;Int>!, glyphInscriptions: UnsafeMutablePointer&lt;NSGlyphInscription>!, elasticBits: UnsafeMutablePointer&lt;ObjCBool>!, bidiLevels: UnsafeMutablePointer&lt;UInt8>!) -> Int

Extracts the information needed to lay out the provided glyphs from the provided range.

Deprecated

func insertGlyph(NSGlyph, atGlyphIndex: Int, characterIndex: Int)

Enables the typesetter to insert a new glyph into the stream.

Deprecated

struct NSTypesetterControlCharacterAction

The following constants are possible values returned by the actionForControlCharacter(at:) method to determine the action associated with a control character.

