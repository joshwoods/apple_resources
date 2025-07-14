

- Notification Center
- NCWidgetProviding
-  widgetDidBeginEditing() Deprecated

Instance Method

# widgetDidBeginEditing()

Called when a user chooses the widget’s begin editing button.

macOS 10.10–11.0Deprecated

``` source
optional func widgetDidBeginEditing()
```

Deprecated

Use WidgetKit instead.

## Discussion

This method can be called when widgetAllowsEditing is true.

## See Also

### Supporting Editing

var widgetAllowsEditing: Bool

A Boolean value indicating whether the widget can be edited by users.

Deprecated

func widgetDidEndEditing()

Called when a widget’s editing session ends.

Deprecated

