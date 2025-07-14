

- AppKit
- NSTableView
-  delegate 

Instance Property

# delegate

The table view’s delegate.

macOS

``` source
@MainActor
weak var delegate: (any NSTableViewDelegate)? { get set }
```

## Discussion

The delegate must conform to the NSTableViewDelegate protocol. Setting the delegate will implicitly reload the table view. Note that in versions of macOS prior to v10.12, the table view did not retain the delegate in a managed memory environment.

### Special Considerations

When you set the table view’s delegate, it is automatically registered for the following notifications with the following delegate methods:

- The notification named selectionDidChangeNotification is configured to notify the delegate’s tableViewSelectionDidChange(_:).

- The notification named columnDidMoveNotification is configured to notify the delegate’s tableViewColumnDidMove(_:).

- The notification named columnDidResizeNotification is configured to notify the delegate’s tableViewColumnDidResize(_:).

- The notification named selectionIsChangingNotification is configured to notify the delegate’s tableViewSelectionIsChanging(_:).

Setting the delegate to `nil` causes these notifications to be disconnected. Rather than setting the delegate to `nil` and listening for notifications (and expecting `NSTableView` to still function correctly) you should instead implement the appropriate delegate method.

