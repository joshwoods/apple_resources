

- UIKit
- UITableViewCell
-  accessoryView 

Instance Property

# accessoryView

The view to use on the right side of the cell, typically as a control, in the table view’s normal state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var accessoryView: UIView? { get set }
```

## Discussion

If the value of this property is not `nil`, the `UITableViewCell` class uses the given view for the accessory view in the table view’s normal (default) state; it ignores the value of the accessoryType property. The provided accessory view can be a framework-provided control or label or a custom view. The accessory view appears in the right side of the cell.

The accessory view cross-fades between normal and editing states if it set for both states; use the editingAccessoryView property to set the accessory view for the cell during editing mode. If this property is not set for both states, the cell is animated to slide in or out, as necessary.

## See Also

### Related Documentation

func willTransition(to: UITableViewCell.StateMask)

Notifies the cell that it’s about to transition to a new cell state.

func didTransition(to: UITableViewCell.StateMask)

Notifies the cell that it transitioned to a new cell state.

### Managing accessory views

var accessoryType: UITableViewCell.AccessoryType

The type of standard accessory view for the cell to use in the table view’s normal state.

var editingAccessoryType: UITableViewCell.AccessoryType

The type of standard accessory view for the cell to use in the table view’s editing state.

var editingAccessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s editing state.

enum AccessoryType

The type of standard accessory control used by a cell.

