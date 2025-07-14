

- AppKit
- NSFontDescriptor
-  NSFontDescriptor.VariationKey 

Structure

# NSFontDescriptor.VariationKey

Constants that can be used as keys to retrieve information about a font descriptor from its variation axis dictionary.

macOS

``` source
struct VariationKey
```

## Discussion

These keys are used with variation.

## Topics

### Variation Keys

static let identifier: NSFontDescriptor.VariationKey

The axis identifier value as a number object.

static let minimumValue: NSFontDescriptor.VariationKey

The minimum axis value as a number object.

static let maximumValue: NSFontDescriptor.VariationKey

The maximum axis value as a number object.

static let defaultValue: NSFontDescriptor.VariationKey

The default axis value as a number object.

static let name: NSFontDescriptor.VariationKey

The localized variation axis name.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Font Attributes

var fontAttributes: [NSFontDescriptor.AttributeName : Any]

The receiver’s dictionary of attributes.

func object(forKey: NSFontDescriptor.AttributeName) -> Any?

Returns the font attribute specified by the given key.

struct AttributeName

Constants for the names of font attributes.

struct SymbolicTraits

A symbolic description of the stylistic aspects of a font.

var matrix: AffineTransform?

The current transform matrix of the receiver.

var pointSize: CGFloat

The point size of the receiver.

var postscriptName: String?

The PostScript name of the receiver.

struct FeatureKey

Constants to use as keys to retrieve information about a font descriptor from its feature dictionary.

typealias NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

var NSFontFamilyClassMask: UInt32

Constant you use to access `NSFontFamilyClass` values in the upper four bits of `NSFontSymbolicTraits`.

Typeface Information

Constants for type faces such as italic or bold.

