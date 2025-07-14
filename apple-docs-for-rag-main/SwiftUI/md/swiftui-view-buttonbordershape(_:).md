

- SwiftUI
- View
-  buttonBorderShape(\_:) 

Instance Method

# buttonBorderShape(\_:)

Sets the border shape for buttons in this view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func buttonBorderShape(_ shape: ButtonBorderShape) -> some View
```

## Parameters 

`shape`  

The shape to use.

## Discussion

The border shape is used to draw the platter for a bordered button. In macOS, some border shapes are only applicable to bordered buttons in widgets.

The border shape affects buttons of the bordered and borderedProminent styles.

## See Also

### Creating buttons

struct Button

A control that initiates an action.

func buttonStyle(_:)

Sets the style for buttons within this view to a button style with a custom appearance and standard interaction behavior.

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

