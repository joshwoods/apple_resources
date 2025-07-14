

- WidgetKit
-  ControlWidgetButton 

Structure

# ControlWidgetButton

A control template representing a button.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
struct ControlWidgetButton where Label : View, ActionLabel : View
```

## Overview

Buttons do not have state and are used for fire-and-forget actions such as playing a sound or launching an app.

## Topics

### Initializers

init(some StringProtocol, action: Action, actionLabel: (Bool) -> ActionLabel)

Creates a button template for a control.

init(LocalizedStringKey, action: Action, actionLabel: (Bool) -> ActionLabel)

Creates a button template for a control.

init(action: Action, label: () -> Label)

Creates a button template for a control.

init(action: Action, label: () -> Label)

Creates a button template for a control that launches an app.

init(action: Action, label: () -> Label, actionLabel: (Bool) -> ActionLabel)

Creates a button template for a control.

## Relationships

### Conforms To

- ControlWidgetTemplate

## See Also

### Controls

Creating controls to perform actions across the system

Perform your app’s actions from Control Center, the Lock Screen, and the Action button.

Adding refinements and configuration to controls

Customize the way controls display across the system and offer people the ability to configure them.

struct ControlWidgetToggle

A control template representing a toggle.

class ControlCenter

An object that contains a list of user-configured controls and is used for reloading controls.

