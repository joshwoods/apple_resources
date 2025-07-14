

- Core Text
-  kCTFontWidthTrait 

Global Variable

# kCTFontWidthTrait

The normalized proportion (width condense or expand) trait from the font traits dictionary.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTFontWidthTrait: CFString
```

## Discussion

This value corresponds to the relative interglyph spacing for a given font. The value returned is a CFNumber object representing a float between `-1.0` and `1.0`. The value of `0.0` corresponds to regular glyph spacing, and negative values represent condensed glyph spacing.

## See Also

### Font Trait Keys

let kCTFontSymbolicTrait: CFString

The symbolic traits value from the font traits dictionary.

let kCTFontWeightTrait: CFString

The normalized weight trait from the font traits dictionary.

let kCTFontSlantTrait: CFString

The normalized slant angle from the font traits dictionary.

