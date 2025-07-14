

- Core Text
-  kCTFontCascadeListAttribute 

Global Variable

# kCTFontCascadeListAttribute

The cascade list used for a font reference.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTFontCascadeListAttribute: CFString
```

## Discussion

The cascade list is a CFArray object containing CTFontDescriptor elements. If unspecified, the global cascade list is used.

## See Also

### Font Attribute Keys

let kCTFontURLAttribute: CFString

The font URL from the font descriptor.

let kCTFontNameAttribute: CFString

The PostScript name from the font descriptor.

let kCTFontDisplayNameAttribute: CFString

The name used to display the font.

let kCTFontFamilyNameAttribute: CFString

The font family name from the font descriptor.

let kCTFontStyleNameAttribute: CFString

The style name of the font.

let kCTFontTraitsAttribute: CFString

The dictionary of font traits for stylistic information.

let kCTFontVariationAttribute: CFString

The dictionary of font variation.

let kCTFontSizeAttribute: CFString

The font point size.

let kCTFontMatrixAttribute: CFString

The font transformation matrix when creating a font.

let kCTFontCharacterSetAttribute: CFString

The Unicode character coverage set for a font reference.

let kCTFontLanguagesAttribute: CFString

A list of covered languages for a font reference.

let kCTFontBaselineAdjustAttribute: CFString

The baseline adjustment for a font reference.

let kCTFontMacintoshEncodingsAttribute: CFString

The Macintosh encodings for a font reference.

let kCTFontFeaturesAttribute: CFString

The font features for a font reference.

let kCTFontFeatureSettingsAttribute: CFString

The font features settings for a font reference.

