

- UIKit
- UIFontDescriptor
-  UIFontDescriptor.Class 

Type Alias

# UIFontDescriptor.Class

Constants that classify certain stylistic qualities of the font.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
typealias Class = Int
```

## Discussion

These values correspond closely to the font class values in the OpenType OS/2 table. The class values are bundled in the upper four bits of the UIFontDescriptor.SymbolicTraits and can be accessed through classMask. For additional information about the specific meaning of each identifier, refer to the OpenType specification.

## See Also

### Constants

struct TextStyle

Constants that describe the preferred styles for fonts.

struct SystemDesign

Constants that describe the system-defined typeface designs.

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

struct AttributeName

Constants that describe font attributes.

struct FeatureKey

Keys for retrieving feature settings.

struct TraitKey

Keys for retrieving the font descriptor’s trait information.

struct Weight

Constants that represent standard typeface styles.

struct Width

