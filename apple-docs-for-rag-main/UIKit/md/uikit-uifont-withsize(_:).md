

- UIKit
- UIFont
-  withSize(\_:) 

Instance Method

# withSize(\_:)

Returns a font object that is the same as the font, but has the specified size.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func withSize(_ fontSize: CGFloat) -> UIFont
```

## Parameters 

`fontSize`  

The desired size (in points) of the new font object. This value must be greater than 0.0.

## Return Value

A font object of the specified size.

## See Also

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

