

- UIKit
- UIFontDescriptor
-  preferredFontDescriptor(withTextStyle:compatibleWith:) 

Type Method

# preferredFontDescriptor(withTextStyle:compatibleWith:)

Returns a font descriptor that contains the text style and the content size category that the provided trait collection specifies.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class func preferredFontDescriptor(
    withTextStyle style: UIFont.TextStyle,
    compatibleWith traitCollection: UITraitCollection?
) -> UIFontDescriptor
```

## Parameters 

`style`  

The text style for which to return a font descriptor.

`traitCollection`  

The trait collection containing the content size category information.

## Return Value

The new font descriptor.

## See Also

### Creating a font descriptor

class func preferredFontDescriptor(withTextStyle: UIFont.TextStyle) -> UIFontDescriptor

Returns a font descriptor that contains the specified text style and the user’s selected content size category.

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

