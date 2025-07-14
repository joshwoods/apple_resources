

- UIKit
- UIFontDescriptor
-  UIFontDescriptor.AttributeName 

Structure

# UIFontDescriptor.AttributeName

Constants that describe font attributes.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 4.0+

``` source
struct AttributeName
```

## Topics

### Constants

static let cascadeList: UIFontDescriptor.AttributeName

The cascading list attribute.

static let characterSet: UIFontDescriptor.AttributeName

The character set attribute.

static let face: UIFontDescriptor.AttributeName

The font face attribute.

static let family: UIFontDescriptor.AttributeName

The font family attribute.

static let featureSettings: UIFontDescriptor.AttributeName

The font feature settings attribute.

static let fixedAdvance: UIFontDescriptor.AttributeName

The glyph advancement attribute.

static let matrix: UIFontDescriptor.AttributeName

The font’s transformation matrix attribute.

static let name: UIFontDescriptor.AttributeName

The font name attribute.

static let size: UIFontDescriptor.AttributeName

The font size attribute.

static let textStyle: UIFontDescriptor.AttributeName

The text style attribute.

static let traits: UIFontDescriptor.AttributeName

The font traits dictionary attribute.

static let visibleName: UIFontDescriptor.AttributeName

The font’s visible name attribute.

### Initializers

init(rawValue: String)

Creates an attribute name with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct TextStyle

Constants that describe the preferred styles for fonts.

struct SystemDesign

Constants that describe the system-defined typeface designs.

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

typealias Class

Constants that classify certain stylistic qualities of the font.

struct FeatureKey

Keys for retrieving feature settings.

struct TraitKey

Keys for retrieving the font descriptor’s trait information.

struct Weight

Constants that represent standard typeface styles.

struct Width

