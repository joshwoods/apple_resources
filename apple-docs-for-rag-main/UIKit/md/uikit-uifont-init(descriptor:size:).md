

- UIKit
- UIFont
-  init(descriptor:size:) 

Initializer

# init(descriptor:size:)

Returns a font that matches the specified font descriptor.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    descriptor: UIFontDescriptor,
    size pointSize: CGFloat
)
```

## Parameters 

`descriptor`  

The font descriptor to match.

`pointSize`  

The size in points to which the font is scaled. If greater than 0.0, it has precedence over `UIFontDescriptorSizeAttribute` in `descriptor`.

## Return Value

A font object for the specified descriptor and size.

## Discussion

In most cases, you can simply use init(name:size:) to create standard scaled fonts.

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

func withSize(CGFloat) -> UIFont

Returns a font object that is the same as the font, but has the specified size.

