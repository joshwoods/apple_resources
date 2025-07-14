

- UIKit
- UIFontDescriptor
-  withSize(\_:) 

Instance Method

# withSize(\_:)

Returns a new font descriptor that’s the same as the existing font descriptor, but with the specified point size.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func withSize(_ newPointSize: CGFloat) -> UIFontDescriptor
```

## Parameters 

`newPointSize`  

The new point size.

## Return Value

The new font descriptor.

## See Also

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

func withSymbolicTraits(UIFontDescriptor.SymbolicTraits) -> UIFontDescriptor?

Returns a new font descriptor that’s the same as the existing font descriptor, but with the specified symbolic traits.

