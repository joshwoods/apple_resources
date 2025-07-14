

- Notification Center
- NCWidgetProviding
-  widgetMarginInsets(forProposedMarginInsets:) Deprecated

Instance Method

# widgetMarginInsets(forProposedMarginInsets:)

Called to let a widget accept the default margin inset values or return custom values to use instead.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 8.0–10.0DeprecatedmacOS 10.10–11.0Deprecated

**iOS, iPadOS**

``` source
optional func widgetMarginInsets(forProposedMarginInsets defaultMarginInsets: UIEdgeInsets) -> UIEdgeInsets
```

**macOS**

``` source
optional func widgetMarginInsets(forProposedMarginInsets defaultMarginInset: NSEdgeInsets) -> NSEdgeInsets
```

Deprecated

Use WidgetKit instead.

## Parameters 

`defaultMarginInsets`  

The default margin insets that are available to the widget.

## Return Value

A value of type UIEdgeInsets that contains the custom margin insets a widget is using instead of the default values.

## Discussion

A widget can implement this method to return custom margin inset values to use instead of the default values specified in `defaultMarginInsets`. (If the widget doesn’t need to use custom values, it should return the unchanged default values in its implementation.) If a widget doesn’t implement this method, it automatically receives the default margin inset values.

## See Also

### Customizing the Display

func widgetActiveDisplayModeDidChange(NCWidgetDisplayMode, withMaximumSize: CGSize)

Called when the active display mode changes.

Deprecated

enum NCWidgetDisplayMode

The modes that can be toggled between when the user activates the More button for a widget running in iOS.

Deprecated

