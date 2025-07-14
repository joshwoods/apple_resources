

- SwiftUI
- Slider
-  init(value:in:label:onEditingChanged:) 

Initializer

# init(value:in:label:onEditingChanged:)

Creates a slider to select a value from a given range, which displays the provided label.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(
    value: Binding,
    in bounds: ClosedRange = 0...1,
    @ViewBuilder label: () -> Label,
    onEditingChanged: @escaping (Bool) -> Void = { _ in }
) where V : BinaryFloatingPoint, V.Stride : BinaryFloatingPoint
```

Available when `Label` conforms to `View` and `ValueLabel` is `EmptyView`.

## Parameters 

`value`  

The selected value within `bounds`.

`bounds`  

The range of the valid values. Defaults to `0...1`.

`label`  

A `View` that describes the purpose of the instance. Not all slider styles show the label, but even in those cases, SwiftUI uses the label for accessibility. For example, VoiceOver uses the label to identify the purpose of the slider.

`onEditingChanged`  

A callback for when editing begins and ends.

## Discussion

The `value` of the created instance is equal to the position of the given value within `bounds`, mapped into `0...1`.

The slider calls `onEditingChanged` when editing begins and ends. For example, on iOS, editing begins when the user starts to drag the thumb along the slider’s track.

## See Also

### Creating a slider with labels

init&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V.Stride, label: () -> Label, onEditingChanged: (Bool) -> Void)

Creates a slider to select a value from a given range, subject to a step increment, which displays the provided label.

init&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, label: () -> Label, minimumValueLabel: () -> ValueLabel, maximumValueLabel: () -> ValueLabel, onEditingChanged: (Bool) -> Void)

Creates a slider to select a value from a given range, which displays the provided labels.

init&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V.Stride, label: () -> Label, minimumValueLabel: () -> ValueLabel, maximumValueLabel: () -> ValueLabel, onEditingChanged: (Bool) -> Void)

Creates a slider to select a value from a given range, subject to a step increment, which displays the provided labels.

