

- AppKit
- NSFontDescriptor
-  NSFontDescriptor.FeatureKey 

Structure

# NSFontDescriptor.FeatureKey

Constants to use as keys to retrieve information about a font descriptor from its feature dictionary.

macOS

``` source
struct FeatureKey
```

## Discussion

These keys are used with featureSettings.

## Topics

### Feature Keys

static let typeIdentifier: NSFontDescriptor.FeatureKey

A key that indicates the type of the font feature.

static let selectorIdentifier: NSFontDescriptor.FeatureKey

A key that indicates the selector of the font feature.

### Initializers

init(String)

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

typealias NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

var NSFontFamilyClassMask: UInt32

Constant you use to access `NSFontFamilyClass` values in the upper four bits of `NSFontSymbolicTraits`.

Typeface Information

Constants for type faces such as italic or bold.

struct VariationKey

Constants that can be used as keys to retrieve information about a font descriptor from its variation axis dictionary.

