

- AppKit
-  NSFontFamilyClass 

Type Alias

# NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

macOS

``` source
typealias NSFontFamilyClass = UInt32
```

## Discussion

These values correspond closely to the font class values in the OpenType OS/2 table. The class values are bundled in the upper four bits of NSFontSymbolicTraits and can be accessed via NSFontFamilyClassMask. For more information about the specific meaning of each identifier, refer to the OpenType specification.

## Topics

### Constants

var NSFontUnknownClass: Int

A font with no design classification.

var NSFontOldStyleSerifsClass: Int

A font where the style is based on the Latin printing style of the 15th to 17th century.

var NSFontTransitionalSerifsClass: Int

A font where the style is based on the Latin printing style of the 18th to 19th century.

var NSFontModernSerifsClass: Int

A font where the style is based on the Latin printing style of the 20th century.

var NSFontClarendonSerifsClass: Int

A font where the style is a variation of the Oldstyle Serifs and the Transitional Serifs.

var NSFontSlabSerifsClass: Int

A font where the style is characterized by serifs with a square transition between the strokes and the serifs (no brackets).

var NSFontFreeformSerifsClass: Int

A font where the style includes serifs, but it expresses a design freedom that does not generally fit within the other serif design classifications.

var NSFontSansSerifClass: Int

A font where the style includes most basic letter forms (excluding Scripts and Ornamentals) that do not have serifs on the strokes.

var NSFontOrnamentalsClass: Int

A font where the style includes highly decorated or stylized character shapes such as those typically used in headlines.

var NSFontScriptsClass: Int

A font where the style is among those typefaces designed to simulate handwriting.

var NSFontSymbolicClass: Int

A font where the style is generally design independent, making it suitable for special characters (icons, dingbats, technical symbols, and so on) that may be used equally well with any font.

## See Also

### Font Data

class NSFont

The representation of a font in an app.

class NSFontDescriptor

A dictionary of attributes that describe a font.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

struct SymbolicTraits

A symbolic description of the stylistic aspects of a font.

class NSFontAssetRequest

typealias NSFontSymbolicTraits

A symbolic description of stylistic aspects of a font.

