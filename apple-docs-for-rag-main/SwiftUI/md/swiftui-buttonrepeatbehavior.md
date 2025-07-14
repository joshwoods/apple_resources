

- SwiftUI
-  ButtonRepeatBehavior 

Structure

# ButtonRepeatBehavior

The options for controlling the repeatability of button actions.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ButtonRepeatBehavior
```

## Overview

Use values of this type with the buttonRepeatBehavior(_:) modifier.

## Topics

### Getting repeat behaviors

static let automatic: ButtonRepeatBehavior

The automatic repeat behavior.

static let enabled: ButtonRepeatBehavior

Repeating button actions will be enabled.

static let disabled: ButtonRepeatBehavior

Repeating button actions will be disabled.

## Relationships

### Conforms To

- Equatable
- Hashable
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

struct ButtonRole

A value that describes the purpose of a button.

