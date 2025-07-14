

- AppKit
- NSFontDescriptor
-  withSize(\_:) 

Instance Method

# withSize(\_:)

Returns a new font descriptor based on the current object, but with the specified point size.

macOS

``` source
func withSize(_ newPointSize: CGFloat) -> NSFontDescriptor
```

## Parameters 

`newPointSize`  

The replacement point size.

## Return Value

The new font descriptor.

## See Also

### Modifying an Existing Font Descriptor

func addingAttributes([NSFontDescriptor.AttributeName : Any]) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified attributes taking precedence over the existing ones.

func withFace(String) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified face.

func withFamily(String) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified font family.

func withMatrix(AffineTransform) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified font matrix.

func withSymbolicTraits(NSFontDescriptor.SymbolicTraits) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified symbolic traits taking precedence over the existing ones.

func withDesign(NSFontDescriptor.SystemDesign) -> Self?

Returns a new font descriptor based on the current object, but with the specified design style.

struct SystemDesign

Constants for font designs, such as monospace, rounded, and serif.

