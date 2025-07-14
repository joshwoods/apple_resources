

- AppKit
- NSTypesetter
-  substituteGlyphs(in:withGlyphs:) Deprecated

Instance Method

# substituteGlyphs(in:withGlyphs:)

Replaces the specified glyphs with specified replacement glyphs.

macOS 10.3–10.13Deprecated

``` source
func substituteGlyphs(
    in glyphRange: NSRange,
    withGlyphs glyphs: UnsafeMutablePointer!
)
```

## Parameters 

`glyphRange`  

The range of glyphs to be substituted.

`glyphs`  

The glyphs to substitute for the glyphs in `glyphRange`.

## Discussion

This method does not alter the glyph-to-character mapping or invalidate layout information.

A subclass can override this method to interact with custom glyph storage.

## See Also

### Deprecated

func actionForControlCharacter(at: Int) -> NSTypesetterControlCharacterAction

Returns the action associated with a control character.

func deleteGlyphs(in: NSRange)

Deletes the specified glyphs from the glyph cache maintained by the layout manager.

Deprecated

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;NSGlyph>!, characterIndexes: UnsafeMutablePointer&lt;Int>!, glyphInscriptions: UnsafeMutablePointer&lt;NSGlyphInscription>!, elasticBits: UnsafeMutablePointer&lt;ObjCBool>!, bidiLevels: UnsafeMutablePointer&lt;UInt8>!) -> Int

Extracts the information needed to lay out the provided glyphs from the provided range.

Deprecated

func insertGlyph(NSGlyph, atGlyphIndex: Int, characterIndex: Int)

Enables the typesetter to insert a new glyph into the stream.

Deprecated

struct NSTypesetterControlCharacterAction

The following constants are possible values returned by the actionForControlCharacter(at:) method to determine the action associated with a control character.

