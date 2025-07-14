

- SwiftUI
- Stepper
-  init(value:in:step:onEditingChanged:label:) Deprecated

Initializer

# init(value:in:step:onEditingChanged:label:)

Creates a stepper configured to increment or decrement a binding to a value using a step value and within a range of values you provide.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 9.0–11.4Deprecated

``` source
nonisolated
init(
    value: Binding,
    in bounds: ClosedRange,
    step: V.Stride = 1,
    onEditingChanged: @escaping (Bool) -> Void = { _ in },
    @ViewBuilder label: () -> Label
) where V : Strideable
```

Available when `Label` conforms to `View`.

Deprecated

Use init(value:in:step:label:onEditingChanged:) instead.

## Parameters 

`value`  

A Binding to a value that you provide.

`bounds`  

A closed range that describes the upper and lower bounds permitted by the stepper.

`step`  

The amount to increment or decrement the stepper when the user clicks or taps the stepper’s increment or decrement buttons, respectively.

`onEditingChanged`  

A closure that’s called when editing begins and ends. For example, on iOS, the user may touch and hold the increment or decrement buttons on a stepper which causes the execution of the `onEditingChanged` closure at the start and end of the gesture.

`label`  

A view describing the purpose of this stepper.

## Discussion

Use this initializer to create a stepper that increments or decrements a binding to value by the step size you provide within the given bounds. By setting the bounds, you ensure that the value never goes below or above the lowest or highest value, respectively.

The example below shows a stepper that displays the effect of incrementing or decrementing a value with the step size of `step` with the bounds defined by `range`:

```
struct StepperView: View {
    @State private var value = 0
    let step = 5
    let range = 1...50

    var body: some View {
        Stepper(value: $value,
                in: range,
                step: step) {
            Text("Current: \(value) in \(range.description) " +
                 "stepping by \(step)")
        }
            .padding(10)
    }
}
```

## See Also

### Deprecated initializers

init&lt;V>(value: Binding&lt;V>, step: V.Stride, onEditingChanged: (Bool) -> Void, label: () -> Label)

Creates a stepper configured to increment or decrement a binding to a value using a step value you provide.

Deprecated

init(onIncrement: (() -> Void)?, onDecrement: (() -> Void)?, onEditingChanged: (Bool) -> Void, label: () -> Label)

Creates a stepper instance that performs the closures you provide when the user increments or decrements the stepper.

Deprecated

