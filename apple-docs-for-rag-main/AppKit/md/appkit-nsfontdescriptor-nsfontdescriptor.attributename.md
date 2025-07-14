

- AppKit
- NSFontDescriptor
-  NSFontDescriptor.AttributeName 

Structure

# NSFontDescriptor.AttributeName

Constants for the names of font attributes.

macOS

``` source
struct AttributeName
```

## Discussion

You can retrieve the values for these attributes using object(forKey:).

## Topics

### Font Attributes

static let family: NSFontDescriptor.AttributeName

An optional string object that specifies the font family.

static let name: NSFontDescriptor.AttributeName

An optional string object that specifies the font name.

static let face: NSFontDescriptor.AttributeName

An optional string object that specifies the font face.

static let size: NSFontDescriptor.AttributeName

An optional floating-point number that specifies the font size.

static let visibleName: NSFontDescriptor.AttributeName

An optional string object that specifies the font’s visible name.

static let matrix: NSFontDescriptor.AttributeName

An affine transform that specifies the font’s transformation matrix.

static let variation: NSFontDescriptor.AttributeName

A dictionary that describes the font’s variation axis.

static let characterSet: NSFontDescriptor.AttributeName

The set of Unicode characters covered by the font.

static let cascadeList: NSFontDescriptor.AttributeName

An array, each member of which is a sub-descriptor.

static let traits: NSFontDescriptor.AttributeName

A dictionary that fully describes the font traits.

static let fixedAdvance: NSFontDescriptor.AttributeName

A floating-point value that overrides the glyph advancement specified by the font.

static let featureSettings: NSFontDescriptor.AttributeName

An array of dictionaries representing non-default font feature settings.

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

struct VariationKey

Constants that can be used as keys to retrieve information about a font descriptor from its variation axis dictionary.

