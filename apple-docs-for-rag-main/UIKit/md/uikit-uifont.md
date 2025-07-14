

- UIKit
-  UIFont 

Class

# UIFont

An object that provides access to the font’s characteristics.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class UIFont
```

## Mentioned in 

Adding a Custom Font to Your App

Scaling Fonts Automatically

## Overview

Use `UIFont` to access your font’s characteristics within your app. It also provides the system with access to the glyph information, used during layout. Font objects are immutable, so it’s safe to use them from multiple threads in your app.

In Objective-C, don’t create font objects using the `alloc` and `init` methods. Instead, use class methods of UIFont, such as preferredFont(forTextStyle:), to look up and retrieve the desired font object. These methods check for an existing font object with the specified characteristics and return it if it exists. Otherwise, they create a new font object based on the desired font characteristics.

## Topics

### Creating Fonts

Scaling Fonts Automatically

Scale text in your interface automatically using Dynamic Type.

Creating self-sizing table view cells

Create table view cells that support Dynamic Type and use system spacing constraints to adjust the spacing surrounding text labels.

class func preferredFont(forTextStyle: UIFont.TextStyle) -> UIFont

Returns an instance of the system font for the specified text style with scaling for the user’s selected content size category.

class func preferredFont(forTextStyle: UIFont.TextStyle, compatibleWith: UITraitCollection?) -> UIFont

Returns an instance of the system font for the appropriate text style and traits.

struct TextStyle

Constants that describe the preferred styles for fonts.

init?(name: String, size: CGFloat)

Creates and returns a font object for the specified font name and size.

init(descriptor: UIFontDescriptor, size: CGFloat)

Returns a font that matches the specified font descriptor.

func withSize(CGFloat) -> UIFont

Returns a font object that is the same as the font, but has the specified size.

### Creating System Fonts

class func systemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in the specified size.

class func systemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the font object for standard interface items in the specified size and weight.

struct Weight

Constants that represent standard typeface styles.

class func systemFont(ofSize: CGFloat, weight: UIFont.Weight, width: UIFont.Width) -> UIFont

struct Width

class func boldSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in boldface type in the specified size.

class func italicSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in italic type in the specified size.

class func monospacedSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the fixed-width font for standard interface text in the specified size.

class func monospacedDigitSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the standard system font with all digits of consistent width.

### Getting the Available Font Names

class var familyNames: [String]

Returns an array of font family names available on the system.

class func fontNames(forFamilyName: String) -> [String]

Returns an array of font names available in a particular font family.

### Getting Font Name Attributes

var familyName: String

The font family name.

var fontName: String

The font face name.

### Getting Font Metrics

var pointSize: CGFloat

The font’s point size, or the effective vertical point size for a font with a nonstandard matrix.

var ascender: CGFloat

The top y-coordinate, offset from the baseline, of the font’s longest ascender.

var descender: CGFloat

The bottom y-coordinate, offset from the baseline, of the font’s longest descender.

var leading: CGFloat

The font’s leading information.

var capHeight: CGFloat

The font’s cap height information.

var xHeight: CGFloat

The x-height of the font.

var lineHeight: CGFloat

The height, in points, of text lines.

### Getting System Font Information

class var labelFontSize: CGFloat

The standard font size, in points, for labels.

class var buttonFontSize: CGFloat

The standard font size, in points, for buttons.

class var smallSystemFontSize: CGFloat

The size, in points, of the standard small system font.

class var systemFontSize: CGFloat

The size, in points, of the standard system font.

### Getting Font Descriptors

var fontDescriptor: UIFontDescriptor

A font descriptor for the font.

class UIFontDescriptor

A collection of attributes that describes a font.

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

class UIFontDescriptor

A collection of attributes that describes a font.

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

class UIFontMetrics

A utility object for obtaining custom fonts that scale to support Dynamic Type.

