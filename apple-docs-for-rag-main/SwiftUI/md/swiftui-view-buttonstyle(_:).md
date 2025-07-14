

- SwiftUI
- View
-  buttonStyle(\_:) 

Instance Method

# buttonStyle(\_:)

Sets the style for buttons within this view to a button style with a custom appearance and standard interaction behavior.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func buttonStyle(_ style: S) -> some View where S : ButtonStyle
```

Show all declarations

## Discussion

Use this modifier to set a specific style for all button instances within a view:

```
HStack {
    Button("Sign In", action: signIn)
    Button("Register", action: register)
}
.buttonStyle(.bordered)
```

You can also use this modifier to set the style for controls that acquire a button style through composition, like the Menu and Toggle views in the following example:

```
VStack {
    Menu("Terms and Conditions") {
        Button("Open in Preview", action: openInPreview)
        Button("Save as PDF", action: saveAsPDF)
    }
    Toggle("Remember Password", isOn: $isToggleOn)
    Toggle("Flag", isOn: $flagged)
    Button("Sign In", action: signIn)
}
.menuStyle(.button)
.toggleStyle(.button)
.buttonStyle(.bordered)
```

The menuStyle(_:) modifier causes the Terms and Conditions menu to render as a button. Similarly, the toggleStyle(_:) modifier causes the two toggles to render as buttons. The button style modifier then causes not only the explicit Sign In Button, but also the menu and toggles with button styling, to render with the bordered button style.

## See Also

### Creating buttons

struct Button

A control that initiates an action.

func buttonBorderShape(ButtonBorderShape) -> some View

Sets the border shape for buttons in this view.

func buttonRepeatBehavior(ButtonRepeatBehavior) -> some View

Sets whether buttons in this view should repeatedly trigger their actions on prolonged interactions.

var buttonRepeatBehavior: ButtonRepeatBehavior

Whether buttons with this associated environment should repeatedly trigger their actions on prolonged interactions.

struct ButtonBorderShape

A shape used to draw a button’s border.

struct ButtonRole

A value that describes the purpose of a button.

struct ButtonRepeatBehavior

The options for controlling the repeatability of button actions.

