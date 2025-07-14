

- SwiftUI
- Stepper
-  init(value:step:onEditingChanged:label:) Deprecated

Initializer

# init(value:step:onEditingChanged:label:)

Creates a stepper configured to increment or decrement a binding to a value using a step value you provide.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 9.0–11.4Deprecated

``` source
nonisolated
init(
    value: Binding,
    step: V.Stride = 1,
    onEditingChanged: @escaping (Bool) -> Void = { _ in },
    @ViewBuilder label: () -> Label
) where V : Strideable
```

Available when `Label` conforms to `View`.

Deprecated

Use init(value:step:label:onEditingChanged:) instead.

## Parameters 

`value`  

The Binding to a value that you provide.

`step`  

The amount to increment or decrement `value` each time the user clicks or taps the stepper’s increment or decrement buttons. Defaults to `1`.

`onEditingChanged`  

A closure that’s called when editing begins and ends. For example, on iOS, the user may touch and hold the increment or decrement buttons on a stepper which causes the execution of the `onEditingChanged` closure at the start and end of the gesture.

`label`  

A view describing the purpose of this stepper.

## Discussion

Use this initializer to create a stepper that increments or decrements a bound value by a specific amount each time the user clicks or taps the stepper’s increment or decrement buttons.

In the example below, a stepper increments or decrements `value` by the `step` value of 5 at each click or tap of the control’s increment or decrement button:

```
struct StepperView: View {
    @State private var value = 1
    let step = 5
    var body: some View {
        Stepper(value: $value,
                step: step) {
            Text("Current value: \(value), step: \(step)")
        }
            .padding(10)
    }
}
```

## See Also

### Deprecated initializers

init&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V.Stride, onEditingChanged: (Bool) -> Void, label: () -> Label)

Creates a stepper configured to increment or decrement a binding to a value using a step value and within a range of values you provide.

Deprecated

init(onIncrement: (() -> Void)?, onDecrement: (() -> Void)?, onEditingChanged: (Bool) -> Void, label: () -> Label)

Creates a stepper instance that performs the closures you provide when the user increments or decrements the stepper.

Deprecated

