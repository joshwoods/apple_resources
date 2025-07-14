

- Core Text
-  kCTLanguageAttributeName 

Global Variable

# kCTLanguageAttributeName

The name of the text language.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTLanguageAttributeName: CFString
```

## Discussion

The value of this attribute must be a CFString containing a language identifier conforming to UTS #35. The default is unset. When this attribute is set to a valid identifier, it will be used to select localized glyphs (if supported by the font), and locale-specific line-breaking rules.

## See Also

### Constants

var ATSFONTREF_DEFINED: Int32

var kBSLNIdeographicHighBaseline: Int

let kCTAdaptiveImageProviderAttributeName: CFString

let kCTBackgroundColorAttributeName: CFString

let kCTBaselineClassAttributeName: CFString

let kCTBaselineClassHanging: CFString

let kCTBaselineClassIdeographicCentered: CFString

let kCTBaselineClassIdeographicHigh: CFString

let kCTBaselineClassIdeographicLow: CFString

let kCTBaselineClassMath: CFString

let kCTBaselineClassRoman: CFString

let kCTBaselineInfoAttributeName: CFString

let kCTBaselineOriginalFont: CFString

let kCTBaselineReferenceFont: CFString

let kCTBaselineReferenceInfoAttributeName: CFString

