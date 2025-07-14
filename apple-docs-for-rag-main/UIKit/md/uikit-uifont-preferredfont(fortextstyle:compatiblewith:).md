

- UIKit
- UIFont
-  preferredFont(forTextStyle:compatibleWith:) 

Type Method

# preferredFont(forTextStyle:compatibleWith:)

Returns an instance of the system font for the appropriate text style and traits.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class func preferredFont(
    forTextStyle style: UIFont.TextStyle,
    compatibleWith traitCollection: UITraitCollection?
) -> UIFont
```

## Parameters 

`style`  

The text style for which to return a font. See UIFont.TextStyle for recognized values.

`traitCollection`  

The traits to use when determining which font to return.

## Return Value

The system font associated with the specified text style and traits.

## Discussion

To create a styled font based on a custom font, use a UIFontMetrics object.

Because fonts are immutable, any element that adjusts for an updated content size category does not modify the font itself. Instead, the element replaces the assigned font with a new instance based on the original settings.

## See Also

### Creating Fonts

Scaling Fonts Automatically

Scale text in your interface automatically using Dynamic Type.

Creating self-sizing table view cells

Create table view cells that support Dynamic Type and use system spacing constraints to adjust the spacing surrounding text labels.

class func preferredFont(forTextStyle: UIFont.TextStyle) -> UIFont

Returns an instance of the system font for the specified text style with scaling for the user’s selected content size category.

struct TextStyle

Constants that describe the preferred styles for fonts.

init?(name: String, size: CGFloat)

Creates and returns a font object for the specified font name and size.

init(descriptor: UIFontDescriptor, size: CGFloat)

Returns a font that matches the specified font descriptor.

func withSize(CGFloat) -> UIFont

Returns a font object that is the same as the font, but has the specified size.

