

- AppKit
- NSFontDescriptor
-  NSFontDescriptor.SymbolicTraits 

Structure

# NSFontDescriptor.SymbolicTraits

A symbolic description of the stylistic aspects of a font.

macOS

``` source
struct SymbolicTraits
```

## Topics

### Symbolic Traits

static var italic: NSFontDescriptor.SymbolicTraits

The font’s style is italic.

static var bold: NSFontDescriptor.SymbolicTraits

The font’s style is boldface.

static var expanded: NSFontDescriptor.SymbolicTraits

The font’s characters have an expanded width.

static var condensed: NSFontDescriptor.SymbolicTraits

The font’s characters have a condensed width.

static var monoSpace: NSFontDescriptor.SymbolicTraits

The font’s characters all have the same width.

static var vertical: NSFontDescriptor.SymbolicTraits

The font uses vertical glyph variants and metrics.

static var UIOptimized: NSFontDescriptor.SymbolicTraits

The font synthesizes appropriate attributes for user interface rendering, such as in control titles, if necessary.

static var tightLeading: NSFontDescriptor.SymbolicTraits

The font uses a leading value that’s less than the default.

static var looseLeading: NSFontDescriptor.SymbolicTraits

The font uses a leading value that’s greater than the default.

static var classMask: NSFontDescriptor.SymbolicTraits

The font family class mask that you use to access font descriptor values.

static var classOldStyleSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 15th to 17th centuries.

static var classTransitionalSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 18th to 19th centuries.

static var classModernSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 20th century.

static var classClarendonSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters include variations of old style and transitional serifs.

static var classSlabSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters use square transitions, without brackets, between strokes and serifs.

static var classFreeformSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters include serifs, and don’t generally fit within other serif design classifications.

static var classSansSerif: NSFontDescriptor.SymbolicTraits

The font’s characters don’t have serifs.

static var classOrnamentals: NSFontDescriptor.SymbolicTraits

The font’s characters use highly decorated or stylized character shapes.

static var classScripts: NSFontDescriptor.SymbolicTraits

The font’s characters simulate handwriting.

static var classSymbolic: NSFontDescriptor.SymbolicTraits

The font’s characters consist mainly of symbols rather than letters and numbers.

### Initializers

init(rawValue: UInt32)

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

### Related Documentation

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

### Font Data

class NSFont

The representation of a font in an app.

class NSFontDescriptor

A dictionary of attributes that describe a font.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

typealias NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

class NSFontAssetRequest

typealias NSFontSymbolicTraits

A symbolic description of stylistic aspects of a font.

