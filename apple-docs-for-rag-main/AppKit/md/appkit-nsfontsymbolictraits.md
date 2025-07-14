

- AppKit
-  NSFontSymbolicTraits 

Type Alias

# NSFontSymbolicTraits

A symbolic description of stylistic aspects of a font.

macOS

``` source
typealias NSFontSymbolicTraits = UInt32
```

## Discussion

The upper 16 bits is used to describe appearance of the font (see NSFontFamilyClass) whereas the lower 16 bits is used for typeface information (see Typeface Information). The font appearance information represented by the upper 16 bits can be used for stylistic font matching. The symbolic traits supersede the existing NSFontTraitMask type used by NSFontManager. The corresponding values are kept compatible between NSFontTraitMask and NSFontSymbolicTraits.

## See Also

### Font Data

class NSFont

The representation of a font in an app.

class NSFontDescriptor

A dictionary of attributes that describe a font.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

typealias NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

struct SymbolicTraits

A symbolic description of the stylistic aspects of a font.

class NSFontAssetRequest

