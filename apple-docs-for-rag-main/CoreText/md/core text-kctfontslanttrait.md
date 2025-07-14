

- Core Text
-  kCTFontSlantTrait 

Global Variable

# kCTFontSlantTrait

The normalized slant angle from the font traits dictionary.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTFontSlantTrait: CFString
```

## Discussion

The value returned is a CFNumber object representing a float value between `-1.0` and `1.0` for normalized slant angle. The value of `0.0` corresponds to 0 degrees clockwise rotation from the vertical and `1.0` corresponds to 30 degrees clockwise rotation.

## See Also

### Font Trait Keys

let kCTFontSymbolicTrait: CFString

The symbolic traits value from the font traits dictionary.

let kCTFontWeightTrait: CFString

The normalized weight trait from the font traits dictionary.

let kCTFontWidthTrait: CFString

The normalized proportion (width condense or expand) trait from the font traits dictionary.

