

- AppKit
-  NSFontDescriptor 

Class

# NSFontDescriptor

A dictionary of attributes that describe a font.

macOS

``` source
class NSFontDescriptor
```

## Overview

A font descriptor can be used to create or modify an NSFont object. The system provides a font matching capability, so that you can partially describe a font by creating a font descriptor with, for example, just a family name. You can then find all the available fonts on the system with a matching family name using matchingFontDescriptors(withMandatoryKeys:).

There are several ways to create a new NSFontDescriptor object. You can use `alloc` and init(fontAttributes:), fontDescriptorWithFontAttributes:, init(name:matrix:), or init(name:size:). to create a font descriptor based on either your custom attributes dictionary or on a specific font’s name and size. Alternatively you can use one of the `fontDescriptor…` instance methods (such as withFace(_:)) to create a modified version of an existing descriptor. The latter methods are useful if you have an existing descriptor and simply want to change one aspect.

All attributes in the attributes dictionary are optional.

## Topics

### Creating a Font Descriptor

class func preferredFontDescriptor(forTextStyle: NSFont.TextStyle, options: [NSFont.TextStyleOptionKey : Any]) -> NSFontDescriptor

Returns a font descriptor that contains the text style.

init(name: String, matrix: AffineTransform)

Returns a font descriptor with the name and matrix attributes set to the given values.

init(name: String, size: CGFloat)

Returns a font descriptor with the name and size attributes set to the given values.

init(fontAttributes: [NSFontDescriptor.AttributeName : Any]?)

Initializes and returns a new font descriptor with the specified attributes.

### Modifying an Existing Font Descriptor

func addingAttributes([NSFontDescriptor.AttributeName : Any]) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified attributes taking precedence over the existing ones.

func withFace(String) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified face.

func withFamily(String) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified font family.

func withMatrix(AffineTransform) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified font matrix.

func withSize(CGFloat) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified point size.

func withSymbolicTraits(NSFontDescriptor.SymbolicTraits) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified symbolic traits taking precedence over the existing ones.

func withDesign(NSFontDescriptor.SystemDesign) -> Self?

Returns a new font descriptor based on the current object, but with the specified design style.

struct SystemDesign

Constants for font designs, such as monospace, rounded, and serif.

### Finding Fonts

func matchingFontDescriptors(withMandatoryKeys: Set&lt;NSFontDescriptor.AttributeName>?) -> [NSFontDescriptor]

Returns all the fonts available on the system whose specified attributes match those of the receiver.

func matchingFontDescriptor(withMandatoryKeys: Set&lt;NSFontDescriptor.AttributeName>?) -> NSFontDescriptor?

Returns a normalized font descriptor whose specified attributes match those of the receiver.

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

struct VariationKey

Constants that can be used as keys to retrieve information about a font descriptor from its variation axis dictionary.

### Getting the Font Traits

var symbolicTraits: NSFontDescriptor.SymbolicTraits

A bit mask that describes the traits of the receiver.

typealias NSFontSymbolicTraits

A symbolic description of stylistic aspects of a font.

struct TraitKey

Constants that can be used as keys to retrieve information about a font descriptor from its trait dictionary.

### Requiring Font Assets

var requiresFontAssetRequest: Bool

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Font Data

class NSFont

The representation of a font in an app.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

typealias NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

struct SymbolicTraits

A symbolic description of the stylistic aspects of a font.

class NSFontAssetRequest

typealias NSFontSymbolicTraits

A symbolic description of stylistic aspects of a font.

