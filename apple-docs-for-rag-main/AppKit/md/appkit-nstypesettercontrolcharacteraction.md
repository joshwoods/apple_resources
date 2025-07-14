

- AppKit
-  NSTypesetterControlCharacterAction 

Structure

# NSTypesetterControlCharacterAction

The following constants are possible values returned by the actionForControlCharacter(at:) method to determine the action associated with a control character.

macOS

``` source
struct NSTypesetterControlCharacterAction
```

## Topics

### Constants

static var zeroAdvancementAction: NSTypesetterControlCharacterAction

Glyphs with this action are filtered out from layout `(notShownAttribute == YES)`.

static var whitespaceAction: NSTypesetterControlCharacterAction

The width for glyphs with this action are determined by boundingBox(forControlGlyphAt:for:proposedLineFragment:glyphPosition:characterIndex:), if the method is implemented; otherwise, same as `NSTypesetterZeroAdvancementAction`.

static var horizontalTabAction: NSTypesetterControlCharacterAction

Treated as tab character.

static var lineBreakAction: NSTypesetterControlCharacterAction

Causes line break.

static var paragraphBreakAction: NSTypesetterControlCharacterAction

Causes paragraph break; the value returned by firstLineHeadIndent is the advancement used for the following glyph.

static var containerBreakAction: NSTypesetterControlCharacterAction

Causes container break.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

func insertGlyph(NSGlyph, atGlyphIndex: Int, characterIndex: Int)

Enables the typesetter to insert a new glyph into the stream.

Deprecated

