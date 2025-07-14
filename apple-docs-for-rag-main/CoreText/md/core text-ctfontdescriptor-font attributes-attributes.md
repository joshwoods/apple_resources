

- Core Text
- CTFontDescriptor
-  Font Attributes 

API Collection

# Font Attributes

The keys for accessing font attributes from a font descriptor.

## Topics

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

let kCTFontCascadeListAttribute: CFString

The cascade list used for a font reference.

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

let kCTFontFixedAdvanceAttribute: CFString

A fixed advance to be used for a font reference.

let kCTFontOrientationAttribute: CFString

The orientation for the glyphs of the font.

let kCTFontFormatAttribute: CFString

The recognized format of the font.

let kCTFontRegistrationScopeAttribute: CFString

The font descriptor’s registration scope.

let kCTFontPriorityAttribute: CFString

The font priority used by font descriptors when resolving duplicates and sorting match results.

let kCTFontEnabledAttribute: CFString

The font enabled state.

let kCTFontDownloadableAttribute: CFString

The font downloadable state.

let kCTFontDownloadedAttribute: CFString

The download state.

## See Also

### Related Documentation

func CTFontDescriptorCopyAttribute(CTFontDescriptor, CFString) -> CFTypeRef?

Returns the value associated with an arbitrary attribute.

func CTFontDescriptorCopyAttributes(CTFontDescriptor) -> CFDictionary

Returns the attributes dictionary of the font descriptor.

func CTFontCopyAttribute(CTFont, CFString) -> CFTypeRef?

Returns the value associated with an arbitrary attribute of the given font.

### Accessing Font Attributes

enum CTFontOrientation

The intended rendering orientation of the font for obtaining glyph metrics.

enum CTFontFormat

The recognized format of the font.

typealias CTFontPriority

The priority of font descriptors when resolving duplicates and sorting match results.

