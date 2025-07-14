

- Notification Center
- NCWidgetProviding
-  widgetDidEndEditing() Deprecated

Instance Method

# widgetDidEndEditing()

Called when a widget’s editing session ends.

macOS 10.10–11.0Deprecated

``` source
optional func widgetDidEndEditing()
```

Deprecated

Use WidgetKit instead.

## Discussion

This method is called when a user chooses the widget’s end editing button or when editing is deactivated because editing begins in a different widget. This method can be called when widgetAllowsEditing is true.

## See Also

### Supporting Editing

var widgetAllowsEditing: Bool

A Boolean value indicating whether the widget can be edited by users.

Deprecated

func widgetDidBeginEditing()

Called when a user chooses the widget’s begin editing button.

Deprecated

