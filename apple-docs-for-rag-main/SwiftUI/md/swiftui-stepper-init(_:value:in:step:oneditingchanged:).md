

- SwiftUI
- Stepper
-  init(\_:value:in:step:onEditingChanged:) 

Initializer

# init(\_:value:in:step:onEditingChanged:)

Creates a stepper instance that increments and decrements a binding to a value, by a step size and within a closed range that you provide.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    _ title: S,
    value: Binding,
    in bounds: ClosedRange,
    step: V.Stride = 1,
    onEditingChanged: @escaping (Bool) -> Void = { _ in }
) where S : StringProtocol, V : Strideable
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`title`  

A string describing the purpose of the stepper.

`value`  

A Binding to a value that your provide.

`bounds`  

A closed range that describes the upper and lower bounds permitted by the stepper.

`step`  

The amount to increment or decrement `value` each time the user clicks or taps the stepper’s increment or decrement button, respectively. Defaults to `1`.

`onEditingChanged`  

A closure that’s called when editing begins and ends. For example, on iOS, the user may touch and hold the increment or decrement buttons on a `Stepper` which causes the execution of the `onEditingChanged` closure at the start and end of the gesture.

## Discussion

Use `Stepper(_:value:in:step:onEditingChanged:)` to create a stepper that increments or decrements a value within a specific range of values by a specific step size. In the example below, a stepper increments or decrements a binding to value over a range of `1...50` by `5` each time the user clicks or taps the stepper’s increment or decrement buttons:

```
struct StepperView: View {
    @State private var value = 0
    let step = 5
    let range = 1...50

    var body: some View {
        Stepper("Current: \(value) in \(range.description) stepping by \(step)",
                value: $value,
                in: range,
                step: step)
            .padding(10)
    }
}
```

## See Also

### Creating a stepper over a range

init&lt;V>(value: Binding&lt;V>, in: ClosedRange&lt;V>, step: V.Stride, label: () -> Label, onEditingChanged: (Bool) -> Void)

Creates a stepper configured to increment or decrement a binding to a value using a step value and within a range of values you provide.

init&lt;F>(value: Binding&lt;F.FormatInput>, in: ClosedRange&lt;F.FormatInput>, step: F.FormatInput.Stride, format: F, label: () -> Label, onEditingChanged: (Bool) -> Void)

Creates a stepper configured to increment or decrement a binding to a value using a step value and within a range of values you provide, displaying its value with an applied format style.

init(_:value:in:step:format:onEditingChanged:)

Creates a stepper instance that increments and decrements a binding to a value, by a step size and within a closed range that you provide, displaying its value with an applied format style.

