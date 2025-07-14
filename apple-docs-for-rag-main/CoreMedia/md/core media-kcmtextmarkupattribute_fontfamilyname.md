

- Core Media
-  kCMTextMarkupAttribute_FontFamilyName 

Global Variable

# kCMTextMarkupAttribute_FontFamilyName

A name of a font family.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMTextMarkupAttribute_FontFamilyName: CFString
```

## Discussion

This attribute’s value must be a `CFString` that holds the family name of an installed font (for example, “Helvetica”) that the system uses to render and/or measure text.

When the system specifies legible output, an attributed string has at most one of kCMTextMarkupAttribute_FontFamilyName or kCMTextMarkupAttribute_GenericFontFamilyName associated with each character.

## See Also

### Fonts

let kCMTextMarkupAttribute_GenericFontFamilyName: CFString

A generic font family name identifier.

let kCMTextMarkupAttribute_BaseFontSizePercentageRelativeToVideoHeight: CFString

A base font size as a percentage of the video height.

let kCMTextMarkupAttribute_RelativeFontSize: CFString

A font size as a percentage of the current default font size.

