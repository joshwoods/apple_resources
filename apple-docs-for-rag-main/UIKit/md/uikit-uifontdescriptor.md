

- UIKit
-  UIFontDescriptor 

Class

# UIFontDescriptor

A collection of attributes that describes a font.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class UIFontDescriptor
```

## Overview

A font descriptor can be used to create or modify a UIFont object. Font descriptors have a font matching capability, so that you can partially describe a font by creating a font descriptor with, for example, just a family name. You can use matchingFontDescriptors(withMandatoryKeys:) to find all the available fonts in the system with a matching family name. Font descriptors can also be archived and unarchived.

There are several ways to create a new UIFontDescriptor object. To take advantage of text styles and respect the user’s current content size category, use preferredFontDescriptor(withTextStyle:). You can also use `alloc` and init(fontAttributes:), fontDescriptorWithFontAttributes:, init(name:matrix:), or init(name:size:) to create a font descriptor based on your custom attributes dictionary or on a specific font’s name and size. Alternatively you can use one of the `fontDescriptor…` instance methods (such as withFace(_:)) to create a modified version of an existing descriptor. The latter methods are useful if you have an existing descriptor and simply want to change one aspect.

All attributes in the attributes dictionary are optional.

For design guidance, see Human Interface Guidelines.

## Topics

### Creating a font descriptor

class func preferredFontDescriptor(withTextStyle: UIFont.TextStyle) -> UIFontDescriptor

Returns a font descriptor that contains the specified text style and the user’s selected content size category.

class func preferredFontDescriptor(withTextStyle: UIFont.TextStyle, compatibleWith: UITraitCollection?) -> UIFontDescriptor

Returns a font descriptor that contains the text style and the content size category that the provided trait collection specifies.

init(name: String, matrix: CGAffineTransform)

Returns a font descriptor with the specified values for the name and matrix dictionary attributes.

init(name: String, size: CGFloat)

Returns a font descriptor with the specified values for the name and size dictionary attributes.

func addingAttributes([UIFontDescriptor.AttributeName : Any]) -> UIFontDescriptor

Returns a new font descriptor that’s the same as the existing descriptor, but with the specified attributes taking precedence over the existing ones.

func withDesign(UIFontDescriptor.SystemDesign) -> UIFontDescriptor?

Returns a new font descriptor that’s the same as the existing descriptor, but with the specified design.

func withFamily(String) -> UIFontDescriptor

Returns a new font descriptor whose attributes are the same as the existing font descriptor, but from the specified family.

func withFace(String) -> UIFontDescriptor

Returns a new font descriptor that’s the same as the existing font descriptor, but with the specified face.

func withMatrix(CGAffineTransform) -> UIFontDescriptor

Returns a new font descriptor that’s the same as the existing font descriptor, but with the specified matrix.

func withSize(CGFloat) -> UIFontDescriptor

Returns a new font descriptor that’s the same as the existing font descriptor, but with the specified point size.

func withSymbolicTraits(UIFontDescriptor.SymbolicTraits) -> UIFontDescriptor?

Returns a new font descriptor that’s the same as the existing font descriptor, but with the specified symbolic traits.

### Initializing a font descriptor

init(fontAttributes: [UIFontDescriptor.AttributeName : Any])

Creates a font descriptor with the specified attributes.

convenience init()

Creates a font descriptor.

init?(coder: NSCoder)

Creates a font descriptor from data in an unarchiver.

### Finding fonts

func matchingFontDescriptors(withMandatoryKeys: Set&lt;UIFontDescriptor.AttributeName>?) -> [UIFontDescriptor]

Returns all the fonts available in the system with specified attributes that match those of the font.

### Querying a font descriptor

var fontAttributes: [UIFontDescriptor.AttributeName : Any]

The font descriptor’s dictionary of attributes.

var matrix: CGAffineTransform

The current transform matrix of the font descriptor.

func object(forKey: UIFontDescriptor.AttributeName) -> Any?

Returns the font attribute that the corresponding key specifies.

var pointSize: CGFloat

The point size of the font descriptor.

var postscriptName: String

The PostScript name of the font descriptor.

var symbolicTraits: UIFontDescriptor.SymbolicTraits

The traits of the font descriptor.

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

### Constants

struct TextStyle

Constants that describe the preferred styles for fonts.

struct SystemDesign

Constants that describe the system-defined typeface designs.

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

typealias Class

Constants that classify certain stylistic qualities of the font.

struct AttributeName

Constants that describe font attributes.

struct FeatureKey

Keys for retrieving feature settings.

struct TraitKey

Keys for retrieving the font descriptor’s trait information.

struct Weight

Constants that represent standard typeface styles.

struct Width

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
- Sendable

## See Also

### Fonts

Scaling Fonts Automatically

Scale text in your interface automatically using Dynamic Type.

Adding a Custom Font to Your App

Add a custom font to your app and use it in your app’s interface.

class UIFont

An object that provides access to the font’s characteristics.

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

class UIFontMetrics

A utility object for obtaining custom fonts that scale to support Dynamic Type.

