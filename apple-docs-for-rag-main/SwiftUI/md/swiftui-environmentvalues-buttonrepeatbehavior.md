

- SwiftUI
- EnvironmentValues
-  buttonRepeatBehavior 

Instance Property

# buttonRepeatBehavior

Whether buttons with this associated environment should repeatedly trigger their actions on prolonged interactions.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var buttonRepeatBehavior: ButtonRepeatBehavior { get }
```

## Discussion

A value of `enabled` means that buttons will be able to repeatedly trigger their action, and `disabled` means they should not. A value of `automatic` means that buttons will defer to default behavior.

## See Also

### Creating buttons

struct Button

A control that initiates an action.

func buttonStyle(_:)

Sets the style for buttons within this view to a button style with a custom appearance and standard interaction behavior.

func buttonBorderShape(ButtonBorderShape) -> some View

Sets the border shape for buttons in this view.

func buttonRepeatBehavior(ButtonRepeatBehavior) -> some View

Sets whether buttons in this view should repeatedly trigger their actions on prolonged interactions.

struct ButtonBorderShape

A shape used to draw a button’s border.

struct ButtonRole

A value that describes the purpose of a button.

struct ButtonRepeatBehavior

The options for controlling the repeatability of button actions.

