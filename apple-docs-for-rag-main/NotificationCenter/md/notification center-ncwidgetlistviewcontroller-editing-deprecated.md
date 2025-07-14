

- Notification Center
- NCWidgetListViewController
-  editing Deprecated

Instance Property

# editing

A Boolean value that indicates whether the list is in editing mode.

macOS 10.10–11.0Deprecated

``` source
@MainActor
var editing: Bool { get set }
```

Deprecated

Use WidgetKit instead.

## Discussion

When you set this property to true, the list view controller can display controls for reordering and removing rows. The default value of this property is false.

## See Also

### Supporting Editing

var showsAddButtonWhenEditing: Bool

A Boolean value that indicates whether an Add (+) button is displayed while the list is in editing mode.

Deprecated

