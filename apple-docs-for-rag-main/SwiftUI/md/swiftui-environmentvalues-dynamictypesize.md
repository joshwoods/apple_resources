

- SwiftUI
- EnvironmentValues
-  dynamicTypeSize 

Instance Property

# dynamicTypeSize

The current Dynamic Type size.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var dynamicTypeSize: DynamicTypeSize { get set }
```

## Discussion

This value changes as the user’s chosen Dynamic Type size changes. The default value is device-dependent.

When limiting the Dynamic Type size, consider if adding a large content view with accessibilityShowsLargeContentViewer() would be appropriate.

On macOS, this value cannot be changed by users and does not affect the text size.

## See Also

### Adjusting text size

func textScale(Text.Scale, isEnabled: Bool) -> some View

Applies a text scale to text in the view.

func dynamicTypeSize(_:)

Sets the Dynamic Type size within the view to the given value.

enum DynamicTypeSize

A Dynamic Type size, which specifies how large scalable content should be.

struct ScaledMetric

A dynamic property that scales a numeric value.

protocol TextVariantPreference

A protocol for controlling the size variant of text views.

struct FixedTextVariant

The default text variant preference that chooses the largest available variant.

struct SizeDependentTextVariant

The size dependent variant preference allows the text to take the available space into account when choosing the variant to display.

