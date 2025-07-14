

- WidgetKit
- ControlWidgetToggle
-  init(isOn:action:label:valueLabel:) 

Initializer

# init(isOn:action:label:valueLabel:)

Creates a toggle template for a control widget.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    isOn: Bool,
    action: Action,
    @ViewBuilder label: @escaping () -> Label,
    @ViewBuilder valueLabel: @escaping (Bool) -> ValueLabel
) where Action : SetValueIntent, Action.ValueType == Bool
```

Available when `Label` conforms to `View` and `ValueLabel` conforms to `View`.

## Parameters 

`isOn`  

A boolean value that describes the current value of the toggle.

`action`  

The action the toggle performs when pressed.

`label`  

A view that renders the toggle’s label.

`valueLabel`  

A view that renders the toggle’s value. The boolean parameter represents the value.

