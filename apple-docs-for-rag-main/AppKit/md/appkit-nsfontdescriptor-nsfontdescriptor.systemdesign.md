

- AppKit
- NSFontDescriptor
-  NSFontDescriptor.SystemDesign 

Structure

# NSFontDescriptor.SystemDesign

Constants for font designs, such as monospace, rounded, and serif.

macOS

``` source
struct SystemDesign
```

## Topics

### Designs

static let `default`: NSFontDescriptor.SystemDesign

The default font design.

static let monospaced: NSFontDescriptor.SystemDesign

A font with a monospace appearance.

static let rounded: NSFontDescriptor.SystemDesign

A font with a rounded appearance.

static let serif: NSFontDescriptor.SystemDesign

A font with a serif design.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

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

func withDesign(NSFontDescriptor.SystemDesign) -> Self?

Returns a new font descriptor based on the current object, but with the specified design style.

