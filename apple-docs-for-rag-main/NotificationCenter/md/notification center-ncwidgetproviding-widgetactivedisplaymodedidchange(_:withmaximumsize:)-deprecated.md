

- Notification Center
- NCWidgetProviding
-  widgetActiveDisplayModeDidChange(\_:withMaximumSize:) Deprecated

Instance Method

# widgetActiveDisplayModeDidChange(\_:withMaximumSize:)

Called when the active display mode changes.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 10.0–14.0Deprecated

``` source
optional func widgetActiveDisplayModeDidChange(
    _ activeDisplayMode: NCWidgetDisplayMode,
    withMaximumSize maxSize: CGSize
)
```

Deprecated

Use WidgetKit instead.

## Parameters 

`activeDisplayMode`  

The new active display mode. See NCWidgetDisplayMode for possible values.

`maxSize`  

A CGSize object that represents the new maximum size this widget can have.

## Discussion

You might implement this method if your widget should change its preferredContentSize value to better accommodate the new display mode.

Widgets displayed as NCWidgetDisplayMode.compact have a fixed size passed in the `maxSize` parameter.

## See Also

### Customizing the Display

func widgetMarginInsets(forProposedMarginInsets: UIEdgeInsets) -> UIEdgeInsets

Called to let a widget accept the default margin inset values or return custom values to use instead.

Deprecated

enum NCWidgetDisplayMode

The modes that can be toggled between when the user activates the More button for a widget running in iOS.

Deprecated

