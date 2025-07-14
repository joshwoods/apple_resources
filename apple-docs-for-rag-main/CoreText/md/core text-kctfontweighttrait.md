

- Core Text
-  kCTFontWeightTrait 

Global Variable

# kCTFontWeightTrait

The normalized weight trait from the font traits dictionary.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTFontWeightTrait: CFString
```

## Discussion

The value returned is a CFNumber representing a float value between `-1.0` and `1.0` for normalized weight. The value of `0.0` corresponds to the regular or medium font weight.

## See Also

### Font Trait Keys

let kCTFontSymbolicTrait: CFString

The symbolic traits value from the font traits dictionary.

let kCTFontWidthTrait: CFString

The normalized proportion (width condense or expand) trait from the font traits dictionary.

let kCTFontSlantTrait: CFString

The normalized slant angle from the font traits dictionary.

