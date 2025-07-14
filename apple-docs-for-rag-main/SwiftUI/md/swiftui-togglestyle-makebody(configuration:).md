

- SwiftUI
- ToggleStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a toggle.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the toggle, including a label and a binding to the toggle’s state.

## Return Value

A view that has behavior and appearance that enables it to function as a Toggle.

## Discussion

Implement this method when you define a custom toggle style that conforms to the ToggleStyle protocol. Use the `configuration` input — a ToggleStyleConfiguration instance — to access the toggle’s label and state. Return a view that has the appearance and behavior of a toggle. For example you can create a toggle that displays a label and a circle that’s either empty or filled with a checkmark:

```
struct ChecklistToggleStyle: ToggleStyle {
    func makeBody(configuration: Configuration) -> some View {
        Button {
            configuration.isOn.toggle()
        } label: {
            HStack {
                Image(systemName: configuration.isOn
                        ? "checkmark.circle.fill"
                        : "circle")
                configuration.label
            }
        }
        .tint(.primary)
        .buttonStyle(.borderless)
    }
}
```

The `ChecklistToggleStyle` toggle style provides a way to both observe and modify the toggle state: the circle fills for the on state, and users can tap or click the toggle to change the state. By using a customized Button to compose the toggle’s body, SwiftUI automatically provides the behaviors that users expect from a control that has button-like characteristics.

You can present a collection of toggles that use this style in a stack:

When updating a view hierarchy, the system calls your implementation of the `makeBody(configuration:)` method for each Toggle instance that uses the associated style.

### Modify the current style

Rather than create an entirely new style, you can alternatively modify a toggle’s current style. Use the init(_:) initializer inside the `makeBody(configuration:)` method to create and modify a toggle based on a `configuration` value. For example, you can create a style that adds padding and a red border to the current style:

```
struct RedBorderToggleStyle: ToggleStyle {
    func makeBody(configuration: Configuration) -> some View {
        Toggle(configuration)
            .padding()
            .border(.red)
    }
}
```

If you create a `redBorder` static variable from this style, you can apply the style to toggles that already use another style, like the built-in switch and button styles:

```
Toggle("Switch", isOn: $isSwitchOn)
    .toggleStyle(.redBorder)
    .toggleStyle(.switch)

Toggle("Button", isOn: $isButtonOn)
    .toggleStyle(.redBorder)
    .toggleStyle(.button)
```

Both toggles appear with the usual styling, each with a red border:

Apply the custom style closer to the toggle than the modified style because SwiftUI evaluates style view modifiers in order from outermost to innermost. If you apply the styles in the other order, the red border style doesn’t have an effect, because the built-in styles override it completely.

## See Also

### Creating custom toggle styles

struct ToggleStyleConfiguration

The properties of a toggle instance.

typealias Configuration

The properties of a toggle instance.

associatedtype Body : View

A view that represents the appearance and interaction of a toggle.

**Required**

