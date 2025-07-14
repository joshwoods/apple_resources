

- SwiftUI
-  SizeDependentTextVariant 

Structure

# SizeDependentTextVariant

The size dependent variant preference allows the text to take the available space into account when choosing the variant to display.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct SizeDependentTextVariant
```

## Relationships

### Conforms To

- Sendable
- TextVariantPreference

## See Also

### Adjusting text size

func textScale(Text.Scale, isEnabled: Bool) -> some View

Applies a text scale to text in the view.

func dynamicTypeSize(_:)

Sets the Dynamic Type size within the view to the given value.

var dynamicTypeSize: DynamicTypeSize

The current Dynamic Type size.

enum DynamicTypeSize

A Dynamic Type size, which specifies how large scalable content should be.

struct ScaledMetric

A dynamic property that scales a numeric value.

protocol TextVariantPreference

A protocol for controlling the size variant of text views.

struct FixedTextVariant

The default text variant preference that chooses the largest available variant.

