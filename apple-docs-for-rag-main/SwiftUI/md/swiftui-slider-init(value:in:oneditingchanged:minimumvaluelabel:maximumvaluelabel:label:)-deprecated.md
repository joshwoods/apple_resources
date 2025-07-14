

- SwiftUI
- Slider
-  init(value:in:onEditingChanged:minimumValueLabel:maximumValueLabel:label:) Deprecated

Initializer

# init(value:in:onEditingChanged:minimumValueLabel:maximumValueLabel:label:)

Creates a slider to select a value from a given range, which displays the provided labels.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
init(
    value: Binding,
    in bounds: ClosedRange = 0...1,
    onEditingChanged: @escaping (Bool) -> Void = { _ in },
    minimumValueLabel: ValueLabel,
    maximumValueLabel: ValueLabel,
    @ViewBuilder label: () -> Label
) where V : BinaryFloatingPoint, V.Stride : BinaryFloatingPoint
```

Available when `Label` conforms to `View` and `ValueLabel` conforms to `View`.

Deprecated

Use init(value:in:label:minimumValueLabel:maximumValueLabel:onEditingChanged:) instead.

## Parameters 

`value`  

The selected value within `bounds`.

`bounds`  

The range of the valid values. Defaults to `0...1`.

`onEditingChanged`  

A callback for when editing begins and ends.

`minimumValueLabel`  

A view that describes `bounds.lowerBound`.

`maximumValueLabel`  

A view that describes `bounds.lowerBound`.

`label`  

A `View` that describes the purpose of the instance. Not all slider styles show the label, but even in those cases, SwiftUI uses the label for accessibility. For example, VoiceOver uses the label to identify the purpose of the slider.

## Discussion

The `value` of the created instance is equal to the position of the given value within `bounds`, mapped into `0...1`.

The slider calls `onEditingChanged` when editing begins and ends. For example, on iOS, editing begins when the user starts to drag the thumb along the slider’s track.

## See Also

### Deprecated initializers

init&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, onEditingChanged: (Bool) -> Void, label: () -> Label)

Creates a slider to select a value from a given range, which displays the provided label.

Deprecated

init&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V.Stride, onEditingChanged: (Bool) -> Void, label: () -> Label)

Creates a slider to select a value from a given range, subject to a step increment, which displays the provided label.

Deprecated

init&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V.Stride, onEditingChanged: (Bool) -> Void, minimumValueLabel: ValueLabel, maximumValueLabel: ValueLabel, label: () -> Label)

Creates a slider to select a value from a given range, subject to a step increment, which displays the provided labels.

Deprecated

