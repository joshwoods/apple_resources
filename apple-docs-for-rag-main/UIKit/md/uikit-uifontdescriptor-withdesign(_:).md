

- UIKit
- UIFontDescriptor
-  withDesign(\_:) 

Instance Method

# withDesign(\_:)

Returns a new font descriptor that’s the same as the existing descriptor, but with the specified design.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 5.2+

``` source
func withDesign(_ design: UIFontDescriptor.SystemDesign) -> UIFontDescriptor?
```

## Parameters 

`design`  

The new system font design.

## Return Value

The new font descriptor, if the original font descriptor is from a system UI font; otherwise, `nil`.

## Discussion

This method changes the design of an existing font descriptor that describes a system UI font — for example, a font descriptor created by methods such as systemFont(ofSize:), preferredFont(forTextStyle:), or preferredFontDescriptor(withTextStyle:). If the original font descriptor doesn’t describe a system font, this method returns `nil`.

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

