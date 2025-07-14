

- SwiftUI
- Stepper
-  init(value:in:step:label:onEditingChanged:) 

Initializer

# init(value:in:step:label:onEditingChanged:)

Creates a stepper configured to increment or decrement a binding to a value using a step value and within a range of values you provide.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    value: Binding,
    in bounds: ClosedRange,
    step: V.Stride = 1,
    @ViewBuilder label: () -> Label,
    onEditingChanged: @escaping (Bool) -> Void = { _ in }
) where V : Strideable
```

Available when `Label` conforms to `View`.

## Parameters 

`value`  

A Binding to a value that you provide.

`bounds`  

A closed range that describes the upper and lower bounds permitted by the stepper.

`step`  

The amount to increment or decrement the stepper when the user clicks or taps the stepper’s increment or decrement buttons, respectively.

`label`  

A view describing the purpose of this stepper.

`onEditingChanged`  

A closure that’s called when editing begins and ends. For example, on iOS, the user may touch and hold the increment or decrement buttons on a stepper which causes the execution of the `onEditingChanged` closure at the start and end of the gesture.

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

### Creating a stepper over a range

init&lt;F>(value: Binding&lt;F.FormatInput>, in: ClosedRange&lt;F.FormatInput>, step: F.FormatInput.Stride, format: F, label: () -> Label, onEditingChanged: (Bool) -> Void)

Creates a stepper configured to increment or decrement a binding to a value using a step value and within a range of values you provide, displaying its value with an applied format style.

init(_:value:in:step:onEditingChanged:)

Creates a stepper instance that increments and decrements a binding to a value, by a step size and within a closed range that you provide.

init(_:value:in:step:format:onEditingChanged:)

Creates a stepper instance that increments and decrements a binding to a value, by a step size and within a closed range that you provide, displaying its value with an applied format style.

