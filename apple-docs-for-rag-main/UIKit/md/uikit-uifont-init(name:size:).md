

- UIKit
- UIFont
-  init(name:size:) 

Initializer

# init(name:size:)

Creates and returns a font object for the specified font name and size.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    name fontName: String,
    size fontSize: CGFloat
)
```

## Parameters 

`fontName`  

The fully specified name of the font. This name incorporates both the font family name and the specific style information for the font.

`fontSize`  

The size (in points) to which the font is scaled. This value must be greater than 0.0.

## Return Value

A font object of the specified name and size.

## Discussion

You can use the fontNames(forFamilyName:) method to retrieve the specific font names for a given font family.

## See Also

### Related Documentation

class var familyNames: [String]

Returns an array of font family names available on the system.

class func fontNames(forFamilyName: String) -> [String]

Returns an array of font names available in a particular font family.

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

init(descriptor: UIFontDescriptor, size: CGFloat)

Returns a font that matches the specified font descriptor.

func withSize(CGFloat) -> UIFont

Returns a font object that is the same as the font, but has the specified size.

