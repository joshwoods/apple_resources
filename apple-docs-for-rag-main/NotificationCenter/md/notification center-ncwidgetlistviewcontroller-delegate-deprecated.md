

- Notification Center
- NCWidgetListViewController
-  delegate Deprecated

Instance Property

# delegate

The list view controller’s delegate or `nil` if the receiver doesn’t have a delegate.

macOS 10.10–11.0Deprecated

``` source
@IBOutlet @MainActor
weak var delegate: (any NCWidgetListViewDelegate)? { get set }
```

Deprecated

Use WidgetKit instead.

## Discussion

A list view controller’s delegate provides a custom view controller for each object in contents. The delegate also performs editing-related functions, such as responding to interaction with an Add (+) button and reordering and removing rows.

To learn about the methods the delegate can implement, see NCWidgetListViewDelegate.

## See Also

### Displaying and Editing List Content

protocol NCWidgetListViewDelegate

The interface for handling content display and editing in the list view of a macOS Today widget.

Deprecated

