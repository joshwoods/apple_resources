

- AppKit
- NSFontDescriptor
-  addingAttributes(\_:) 

Instance Method

# addingAttributes(\_:)

Returns a new font descriptor based on the current object, but with the specified attributes taking precedence over the existing ones.

macOS

``` source
func addingAttributes(_ attributes: [NSFontDescriptor.AttributeName : Any] = [:]) -> NSFontDescriptor
```

## Parameters 

`attributes`  

The replacement attributes for the new font descriptor.

## Return Value

The new font descriptor.

## See Also

### Modifying an Existing Font Descriptor

func withFace(String) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified face.

func withFamily(String) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified font family.

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

