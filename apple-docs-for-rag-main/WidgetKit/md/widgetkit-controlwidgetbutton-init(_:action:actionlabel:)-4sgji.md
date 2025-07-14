

- WidgetKit
- ControlWidgetButton
-  init(\_:action:actionLabel:) 

Initializer

# init(\_:action:actionLabel:)

Creates a button template for a control.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    _ title: some StringProtocol,
    action: Action,
    @ViewBuilder actionLabel: @escaping (Bool) -> ActionLabel
) where Action : AppIntent
```

Available when `Label` is `Text` and `ActionLabel` conforms to `View`.

## Parameters 

`title`  

A string to display as the title of the button.

`action`  

The action your button performs when pressed.

`actionLabel`  

A view that is rendered when the button’s action is performed.

## Discussion

Use the action label to additionally customize the appearance of this control button while its action is performed

```
ControlWidgetButton(
    configuration.actionName,
    action: OpenTrunkIntent(configuration.id)
) { isActive in
    Image(systemName: "car.side.rear.open.crop")
    if isActive {
        Text("Opening...")
    }
}
```

The example above produces a control button that in control center will display the value of `actionName` as its title and the provided SF symbol. While the control is performing its action it will show the “Opening…” subtitle.

