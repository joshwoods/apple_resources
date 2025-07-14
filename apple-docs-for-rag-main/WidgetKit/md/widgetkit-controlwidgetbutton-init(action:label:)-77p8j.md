

- WidgetKit
- ControlWidgetButton
-  init(action:label:) 

Initializer

# init(action:label:)

Creates a button template for a control.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    action: Action,
    @ViewBuilder label: @escaping () -> Label
) where ActionLabel == ControlWidgetButtonDefaultActionLabel, Action : AppIntent
```

Available when `Label` conforms to `View` and `ActionLabel` conforms to `View`.

## Parameters 

`action`  

The action your button performs when pressed.

`label`  

A view that renders the button.

