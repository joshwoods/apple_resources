

- SwiftUI
-  ScaledMetric 

Structure

# ScaledMetric

A dynamic property that scales a numeric value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@propertyWrapper
struct ScaledMetric where Value : BinaryFloatingPoint
```

## Mentioned in 

Applying custom fonts to text

## Topics

### Creating the metric

init(wrappedValue: Value)

Creates the scaled metric with an unscaled value using the default scaling.

init(wrappedValue: Value, relativeTo: Font.TextStyle)

Creates the scaled metric with an unscaled value and a text style to scale relative to.

### Getting the metric

var wrappedValue: Value

The value scaled based on the current environment.

## Relationships

### Conforms To

- DynamicProperty
- Sendable

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

protocol TextVariantPreference

A protocol for controlling the size variant of text views.

struct FixedTextVariant

The default text variant preference that chooses the largest available variant.

struct SizeDependentTextVariant

The size dependent variant preference allows the text to take the available space into account when choosing the variant to display.

