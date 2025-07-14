

- AppKit
- NSTypesetter
-  actionForControlCharacter(at:) 

Instance Method

# actionForControlCharacter(at:)

Returns the action associated with a control character.

macOS

``` source
func actionForControlCharacter(at charIndex: Int) -> NSTypesetterControlCharacterAction
```

## Parameters 

`charIndex`  

The index of the control character.

## Return Value

The action associated with the control character at `charIndex`.

## See Also

### Deprecated

func deleteGlyphs(in: NSRange)

Deletes the specified glyphs from the glyph cache maintained by the layout manager.

Deprecated

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

