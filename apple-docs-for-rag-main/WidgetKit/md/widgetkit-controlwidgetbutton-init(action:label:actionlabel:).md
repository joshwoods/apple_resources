

- WidgetKit
- ControlWidgetButton
-  init(action:label:actionLabel:) 

Initializer

# init(action:label:actionLabel:)

Creates a button template for a control.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    action: Action,
    @ViewBuilder label: @escaping () -> Label,
    @ViewBuilder actionLabel: @escaping (Bool) -> ActionLabel
) where Action : AppIntent
```

Available when `Label` conforms to `View` and `ActionLabel` conforms to `View`.

## Parameters 

`action`  

The action your button performs when pressed.

`label`  

A view that renders the button.

`actionLabel`  

A view that is rendered when the button’s action is performed

## Discussion

Use the action label to additionally customize the appearance of this control button while its action is performed

```
ControlWidgetButton(action: OpenTrunkIntent()) {
    Label("Open Trunk", systemImage: "car.side.rear.open.crop")
} actionLabel: { isActive in
    if isActive {
        Text("Opening…")
    }
}
```

The example above produces a control button that in control center will display “Open Trunk” as its title and the provided SF symbol. While the control is performing its action it will show the “Opening…” subtitle.

