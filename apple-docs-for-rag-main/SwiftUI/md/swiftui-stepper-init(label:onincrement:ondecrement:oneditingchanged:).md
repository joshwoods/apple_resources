

- SwiftUI
- Stepper
-  init(label:onIncrement:onDecrement:onEditingChanged:) 

Initializer

# init(label:onIncrement:onDecrement:onEditingChanged:)

Creates a stepper instance that performs the closures you provide when the user increments or decrements the stepper.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 9.0+

``` source
init(
    @ViewBuilder label: () -> Label,
    onIncrement: (() -> Void)?,
    onDecrement: (() -> Void)?,
    onEditingChanged: @escaping (Bool) -> Void = { _ in }
)
```

## Parameters 

`label`  

A view describing the purpose of this stepper.

`onIncrement`  

The closure to execute when the user clicks or taps the control’s plus button.

`onDecrement`  

The closure to execute when the user clicks or taps the control’s minus button.

`onEditingChanged`  

A closure called when editing begins and ends. For example, on iOS, the user may touch and hold the increment or decrement buttons on a `Stepper` which causes the execution of the `onEditingChanged` closure at the start and end of the gesture.

## Discussion

Use this initializer to create a control with a custom title that executes closures you provide when the user clicks or taps the stepper’s increment or decrement buttons.

The example below uses an array that holds a number of Color values, a local state variable, `value`, to set the control’s background color, and title label. When the user clicks or taps on the stepper’s increment or decrement buttons SwiftUI executes the relevant closure that updates `value`, wrapping the `value` to prevent overflow. SwiftUI then re-renders the view, updating the text and background color to match the current index:

```
struct StepperView: View {
    @State private var value = 0
    let colors: [Color] = [.orange, .red, .gray, .blue, .green,
                           .purple, .pink]

    func incrementStep() {
        value += 1
        if value >= colors.count { value = 0 }
    }

    func decrementStep() {
        value -= 1
        if value 

}

## See Also

### Creating a stepper with change behavior

init(_:onIncrement:onDecrement:onEditingChanged:)

Creates a stepper that uses a title key and executes the closures you provide when the user clicks or taps the stepper’s increment and decrement buttons.

