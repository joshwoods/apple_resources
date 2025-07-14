

- Notification Center
- NCWidgetProviding
-  widgetAllowsEditing Deprecated

Instance Property

# widgetAllowsEditing

A Boolean value indicating whether the widget can be edited by users.

macOS 10.10–11.0Deprecated

``` source
optional var widgetAllowsEditing: Bool { get }
```

Deprecated

Use WidgetKit instead.

## Discussion

When a widget that supports editing sets this property to true, it automatically gets a system-provided button in its header area that users choose to begin or end editing. The default value of this property is false.

## See Also

### Supporting Editing

func widgetDidBeginEditing()

Called when a user chooses the widget’s begin editing button.

Deprecated

func widgetDidEndEditing()

Called when a widget’s editing session ends.

Deprecated

