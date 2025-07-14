

- SwiftUI
-  TextVariantPreference 

Protocol

# TextVariantPreference

A protocol for controlling the size variant of text views.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol TextVariantPreference
```

## Topics

### Type Properties

static var fixed: FixedTextVariant

The default text variant preference. It always chooses the largest available variant.

static var sizeDependent: SizeDependentTextVariant

The size dependent preference allows the text to take the available space into account when choosing the size variant to display.

## Relationships

### Conforming Types

- FixedTextVariant
- SizeDependentTextVariant

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

struct FixedTextVariant

The default text variant preference that chooses the largest available variant.

struct SizeDependentTextVariant

The size dependent variant preference allows the text to take the available space into account when choosing the variant to display.

