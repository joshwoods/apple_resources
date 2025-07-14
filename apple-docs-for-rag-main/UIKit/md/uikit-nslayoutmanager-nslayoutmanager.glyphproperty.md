

- UIKit
- NSLayoutManager
-  NSLayoutManager.GlyphProperty 

Structure

# NSLayoutManager.GlyphProperty

Glyph properties.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
struct GlyphProperty
```

## Topics

### Glyph properties

static var null: NSLayoutManager.GlyphProperty

The null glyph, which the layout manager ignores.

static var controlCharacter: NSLayoutManager.GlyphProperty

A glyph representing a control character.

static var elastic: NSLayoutManager.GlyphProperty

A glyph with a changeable width, such as a white space character.

static var nonBaseCharacter: NSLayoutManager.GlyphProperty

A glyph that combines several properties.

### Initializers

init(rawValue: Int)

Creates a new instance with the specified raw value.

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

### Accessing glyphs

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;CGGlyph>?, properties: UnsafeMutablePointer&lt;NSLayoutManager.GlyphProperty>?, characterIndexes: UnsafeMutablePointer&lt;Int>?, bidiLevels: UnsafeMutablePointer&lt;UInt8>?) -> Int

Fills a passed-in buffer with a sequence of glyphs.

func cgGlyph(at: Int) -> CGGlyph

Returns the glyph at the specified index.

func cgGlyph(at: Int, isValidIndex: UnsafeMutablePointer&lt;ObjCBool>?) -> CGGlyph

Returns the glyph at the specified index along with information about whether the glyph index is valid.

func setGlyphs(UnsafePointer&lt;CGGlyph>, properties: UnsafePointer&lt;NSLayoutManager.GlyphProperty>, characterIndexes: UnsafePointer&lt;Int>, font: UIFont, forGlyphRange: NSRange)

Stores the initial glyphs and glyph properties for a character range.

func characterIndexForGlyph(at: Int) -> Int

Returns the index in the text storage for the first character of the specified glyph.

func glyphIndexForCharacter(at: Int) -> Int

Returns the index of the first glyph of the character at the specified index.

func isValidGlyphIndex(Int) -> Bool

Indicates whether the specified index refers to a valid glyph.

var numberOfGlyphs: Int

The number of glyphs in the layout manager.

func propertyForGlyph(at: Int) -> NSLayoutManager.GlyphProperty

Returns the glyph property of the glyph at the specified index.

