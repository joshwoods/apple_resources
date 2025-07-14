

- AppKit
- NSFontDescriptor
-  withDesign(\_:) 

Instance Method

# withDesign(\_:)

Returns a new font descriptor based on the current object, but with the specified design style.

macOS 10.15+

``` source
func withDesign(_ design: NSFontDescriptor.SystemDesign) -> Self?
```

## Parameters 

`design`  

The replacement design style for the font. For a list of possible values, see `UIFontDescriptor.SystemDesign`.

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

func withSize(CGFloat) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified point size.

func withSymbolicTraits(NSFontDescriptor.SymbolicTraits) -> NSFontDescriptor

Returns a new font descriptor based on the current object, but with the specified symbolic traits taking precedence over the existing ones.

struct SystemDesign

Constants for font designs, such as monospace, rounded, and serif.

