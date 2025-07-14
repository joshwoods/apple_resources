

- SwiftUI
- Slider
-  init(value:in:step:onEditingChanged:) 

Initializer

# init(value:in:step:onEditingChanged:)

Creates a slider to select a value from a given range, subject to a step increment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(
    value: Binding,
    in bounds: ClosedRange,
    step: V.Stride = 1,
    onEditingChanged: @escaping (Bool) -> Void = { _ in }
) where V : BinaryFloatingPoint, V.Stride : BinaryFloatingPoint
```

Available when `Label` is `EmptyView` and `ValueLabel` is `EmptyView`.

## Parameters 

`value`  

The selected value within `bounds`.

`bounds`  

The range of the valid values.

`step`  

The distance between each valid value.

`onEditingChanged`  

A callback for when editing begins and ends.

## Discussion

The `value` of the created instance is equal to the position of the given value within `bounds`, mapped into `0...1`.

The slider calls `onEditingChanged` when editing begins and ends. For example, on iOS, editing begins when the user starts to drag the thumb along the slider’s track.

## See Also

### Creating a slider

init&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, onEditingChanged: (Bool) -> Void)

Creates a slider to select a value from a given range.

