

- SwiftUI
-  ButtonBorderShape 

Structure

# ButtonBorderShape

A shape used to draw a button’s border.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ButtonBorderShape
```

## Overview

Use the buttonBorderShape(_:) view modifier to apply the shape to bordered buttons within a view hierarchy.

## Topics

### Getting border shapes

static let automatic: ButtonBorderShape

A shape that defers to the system to determine an appropriate shape for the given context and platform.

static let capsule: ButtonBorderShape

A capsule shape.

static let circle: ButtonBorderShape

A circular shape.

static let roundedRectangle: ButtonBorderShape

A rounded rectangle shape.

static func roundedRectangle(radius: CGFloat) -> ButtonBorderShape

A rounded rectangle shape.

## Relationships

### Conforms To

- Animatable
- Copyable
- Equatable
- InsettableShape
- Sendable
- Shape
- View

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

struct ButtonRole

A value that describes the purpose of a button.

struct ButtonRepeatBehavior

The options for controlling the repeatability of button actions.

