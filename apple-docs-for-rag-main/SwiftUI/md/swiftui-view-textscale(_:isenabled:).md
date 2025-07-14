

- SwiftUI
- View
-  textScale(\_:isEnabled:) 

Instance Method

# textScale(\_:isEnabled:)

Applies a text scale to text in the view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func textScale(
    _ scale: Text.Scale,
    isEnabled: Bool = true
) -> some View
```

## Parameters 

`scale`  

The text scale to apply.

`isEnabled`  

If true the text scale is applied; otherwise text scale is unchanged.

## Return Value

A view with the specified text scale applied.

## See Also

### Adjusting text size

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

struct SizeDependentTextVariant

The size dependent variant preference allows the text to take the available space into account when choosing the variant to display.

