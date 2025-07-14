

- SwiftUI
-  ButtonRole 

Structure

# ButtonRole

A value that describes the purpose of a button.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ButtonRole
```

## Overview

A button role provides a description of a button’s purpose. For example, the destructive role indicates that a button performs a destructive action, like delete user data:

```
Button("Delete", role: .destructive) { delete() }
```

## Topics

### Getting button roles

static let cancel: ButtonRole

A role that indicates a button that cancels an operation.

static let destructive: ButtonRole

A role that indicates a destructive button.

## Relationships

### Conforms To

- Equatable
- Sendable

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

var buttonRepeatBehavior: ButtonRepeatBehavior

Whether buttons with this associated environment should repeatedly trigger their actions on prolonged interactions.

struct ButtonBorderShape

A shape used to draw a button’s border.

struct ButtonRepeatBehavior

The options for controlling the repeatability of button actions.

