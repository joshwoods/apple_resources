

- AppKit
- NSFontDescriptor
-  withFamily(\_:) 

Instance Method

# withFamily(\_:)

Returns a new font descriptor based on the current object, but with the specified font family.

macOS

``` source
func withFamily(_ newFamily: String) -> NSFontDescriptor
```

## Parameters 

`newFamily`  

The replacement font family.

## Return Value

The new font descriptor.

## See Also

### Modifying an Existing Font Descriptor

func addingAttributes([NSFontDescriptor.AttributeName : Any]) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified attributes taking precedence over the existing ones.

func withFace(String) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified face.

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

