

- WidgetKit
- ControlWidgetToggle
-  init(isOn:action:label:) 

Initializer

# init(isOn:action:label:)

Creates a toggle template for a control widget.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    isOn: Bool,
    action: Action,
    @ViewBuilder label: @escaping () -> Label
) where ValueLabel == ControlWidgetToggleDefaultLabel, Action : SetValueIntent, Action.ValueType == Bool
```

Available when `Label` conforms to `View` and `ValueLabel` conforms to `View`.

## Parameters 

`isOn`  

A boolean value that describes the current value of the toggle.

`action`  

The action the toggle performs when pressed.

`label`  

A view that renders the toggle’s label.

## Discussion

The toggle will use “On” and “Off” as default value label.

