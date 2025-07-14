

- FinanceKitUI
- TransactionPicker
-  controlWidgetStatus(\_:) 

Instance Method

# controlWidgetStatus(\_:)

The status of the control described by the modified label.

FinanceKitUISwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func controlWidgetStatus(_ status: S) -> some View where S : StringProtocol
```

## Parameters 

`status`  

The status to display.

## Discussion

This text will appear in Control Center when your control’s state changes. You can customize the text by applying this modifier to the control’s value label:

```
// Status Text: "Do Not Disturb Until This Evening" / "Do Not Disturb Disabled"
ControlWidgetToggle("Do Not Disturb", ...) { isOn in
    Image(systemName: "moon")
        .controlWidgetStatus(isOn ? "Do Not Disturb Until This Evening" : "Do Not Disturb Disabled")
}
```

