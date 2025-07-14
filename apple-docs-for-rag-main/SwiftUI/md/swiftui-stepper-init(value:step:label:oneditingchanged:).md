

- SwiftUI
- Stepper
-  init(value:step:label:onEditingChanged:) 

Initializer

# init(value:step:label:onEditingChanged:)

Creates a stepper configured to increment or decrement a binding to a value using a step value you provide.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    value: Binding,
    step: V.Stride = 1,
    @ViewBuilder label: () -> Label,
    onEditingChanged: @escaping (Bool) -> Void = { _ in }
) where V : Strideable
```

Available when `Label` conforms to `View`.

## Parameters 

`value`  

The Binding to a value that you provide.

`step`  

The amount to increment or decrement `value` each time the user clicks or taps the stepper’s increment or decrement buttons. Defaults to `1`.

`label`  

A view describing the purpose of this stepper.

`onEditingChanged`  

A closure that’s called when editing begins and ends. For example, on iOS, the user may touch and hold the increment or decrement buttons on a stepper which causes the execution of the `onEditingChanged` closure at the start and end of the gesture.

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

### Creating a stepper

init&lt;F>(value: Binding&lt;F.FormatInput>, step: F.FormatInput.Stride, format: F, label: () -> Label, onEditingChanged: (Bool) -> Void)

Creates a stepper configured to increment or decrement a binding to a value using a step value you provide, displaying its value with an applied format style.

init(_:value:step:onEditingChanged:)

Creates a stepper with a title and configured to increment and decrement a binding to a value and step amount you provide.

init(_:value:step:format:onEditingChanged:)

Creates a stepper with a title key and configured to increment and decrement a binding to a value and step amount you provide, displaying its value with an applied format style.

