

- Core Media
-  kCMTextMarkupAttribute_GenericFontFamilyName 

Global Variable

# kCMTextMarkupAttribute_GenericFontFamilyName

A generic font family name identifier.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMTextMarkupAttribute_GenericFontFamilyName: CFString
```

## Discussion

This attribute’s value must be one of the constants listed below. You need to map generic fonts to the family name of an installed font before rendering and/or measuring text (see Media Accessibility).

When the system specifies legible output, an attributed string has at most one of kCMTextMarkupAttribute_FontFamilyName or kCMTextMarkupAttribute_GenericFontFamilyName associated with each character.

## Topics

### Font Names

let kCMTextMarkupGenericFontName_Default: CFString

The default font.

let kCMTextMarkupGenericFontName_Serif: CFString

A font with serifs.

let kCMTextMarkupGenericFontName_SansSerif: CFString

A font without serifs.

let kCMTextMarkupGenericFontName_Monospace: CFString

A monospaced font with or without serifs.

let kCMTextMarkupGenericFontName_MonospaceSerif: CFString

A monospaced font with serifs.

let kCMTextMarkupGenericFontName_MonospaceSansSerif: CFString

A monospaced font without serifs.

let kCMTextMarkupGenericFontName_ProportionalSerif: CFString

A proportional font with serifs.

let kCMTextMarkupGenericFontName_ProportionalSansSerif: CFString

A proportional font without serifs.

let kCMTextMarkupGenericFontName_SmallCapital: CFString

A font with lowercase letters set as small capital letters.

let kCMTextMarkupGenericFontName_Casual: CFString

A casual font.

let kCMTextMarkupGenericFontName_Cursive: CFString

A cursive font.

let kCMTextMarkupGenericFontName_Fantasy: CFString

A fantasy font.

## See Also

### Fonts

let kCMTextMarkupAttribute_FontFamilyName: CFString

A name of a font family.

let kCMTextMarkupAttribute_BaseFontSizePercentageRelativeToVideoHeight: CFString

A base font size as a percentage of the video height.

let kCMTextMarkupAttribute_RelativeFontSize: CFString

A font size as a percentage of the current default font size.

