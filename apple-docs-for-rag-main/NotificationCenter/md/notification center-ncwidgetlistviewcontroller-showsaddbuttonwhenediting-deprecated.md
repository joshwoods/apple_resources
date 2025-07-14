

- Notification Center
- NCWidgetListViewController
-  showsAddButtonWhenEditing Deprecated

Instance Property

# showsAddButtonWhenEditing

A Boolean value that indicates whether an Add (+) button is displayed while the list is in editing mode.

macOS 10.10–11.0Deprecated

``` source
@MainActor
var showsAddButtonWhenEditing: Bool { get set }
```

Deprecated

Use WidgetKit instead.

## Discussion

If users click the Add (+) button while in editing mode, the button’s action send the widgetListPerformAddAction(_:) message to the delegate.

## See Also

### Supporting Editing

var editing: Bool

A Boolean value that indicates whether the list is in editing mode.

Deprecated

