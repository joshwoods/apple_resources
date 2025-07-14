

- WidgetKit
-  ControlWidgetToggle 

Structure

# ControlWidgetToggle

A control template representing a toggle.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
struct ControlWidgetToggle where Label : View, ValueLabel : View
```

## Overview

Toggles are controls that have two states, “off” and “on”.

## Topics

### Initializers

init(some StringProtocol, isOn: Bool, action: Action, valueLabel: (Bool) -> ValueLabel)

Creates a toggle template for a control widget.

init(LocalizedStringKey, isOn: Bool, action: Action, valueLabel: (Bool) -> ValueLabel)

Creates a toggle template for a control widget.

init(isOn: Bool, action: Action, label: () -> Label)

Creates a toggle template for a control widget.

init(isOn: Bool, action: Action, label: () -> Label, valueLabel: (Bool) -> ValueLabel)

Creates a toggle template for a control widget.

## Relationships

### Conforms To

- ControlWidgetTemplate

## See Also

### Controls

Creating controls to perform actions across the system

Perform your app’s actions from Control Center, the Lock Screen, and the Action button.

Adding refinements and configuration to controls

Customize the way controls display across the system and offer people the ability to configure them.

struct ControlWidgetButton

A control template representing a button.

class ControlCenter

An object that contains a list of user-configured controls and is used for reloading controls.

