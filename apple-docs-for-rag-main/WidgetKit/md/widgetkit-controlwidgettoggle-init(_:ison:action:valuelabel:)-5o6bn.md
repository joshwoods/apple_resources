

- WidgetKit
- ControlWidgetToggle
-  init(\_:isOn:action:valueLabel:) 

Initializer

# init(\_:isOn:action:valueLabel:)

Creates a toggle template for a control widget.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    _ titleKey: LocalizedStringKey,
    isOn: Bool,
    action: Action,
    @ViewBuilder valueLabel: @escaping (Bool) -> ValueLabel
) where Action : SetValueIntent, Action.ValueType == Bool
```

Available when `Label` is `Text` and `ValueLabel` conforms to `View`.

## Parameters 

`titleKey`  

The key to a localized string to display as the title of the toggle.

`isOn`  

A boolean value that describes the current value of the toggle.

`action`  

The action the toggle performs when pressed.

`valueLabel`  

A view that renders the toggle’s value. The boolean parameter represents the value.

