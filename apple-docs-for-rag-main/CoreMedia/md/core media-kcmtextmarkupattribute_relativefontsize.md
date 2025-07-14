

- Core Media
-  kCMTextMarkupAttribute_RelativeFontSize 

Global Variable

# kCMTextMarkupAttribute_RelativeFontSize

A font size as a percentage of the current default font size.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMTextMarkupAttribute_RelativeFontSize: CFString
```

## Discussion

This attribute’s value must be a non-negative `CFNumber`. This is a number holding a percentage of the size of the calculated default font size. A value of `120` indicates 20% larger than the default font size. A value of `80` indicates 80% of the default font size. The default value of `100` indicates no size difference.

## See Also

### Fonts

let kCMTextMarkupAttribute_FontFamilyName: CFString

A name of a font family.

let kCMTextMarkupAttribute_GenericFontFamilyName: CFString

A generic font family name identifier.

let kCMTextMarkupAttribute_BaseFontSizePercentageRelativeToVideoHeight: CFString

A base font size as a percentage of the video height.

