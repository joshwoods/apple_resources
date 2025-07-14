

- AppKit
- NSFontDescriptor
-  postscriptName 

Instance Property

# postscriptName

The PostScript name of the receiver.

macOS

``` source
var postscriptName: String? { get }
```

## See Also

### Related Documentation

var symbolicTraits: NSFontDescriptor.SymbolicTraits

A bit mask that describes the traits of the receiver.

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

