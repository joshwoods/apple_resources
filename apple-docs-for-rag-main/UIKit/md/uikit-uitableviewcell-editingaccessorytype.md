

- UIKit
- UITableViewCell
-  editingAccessoryType 

Instance Property

# editingAccessoryType

The type of standard accessory view for the cell to use in the table view’s editing state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var editingAccessoryType: UITableViewCell.AccessoryType { get set }
```

## Discussion

The accessory view appears in the right side of the cell when the table view is in editing mode. The standard accessory views include the disclosure chevron; for a description of valid constants, see UITableViewCell.AccessoryType. The default is UITableViewCell.AccessoryType.none. If a custom accessory view for editing mode is set through the editingAccessoryView property, the value of this property is ignored. If the cell is enabled and the accessory type is UITableViewCell.AccessoryType.detailDisclosureButton, the accessory view tracks touches and, when tapped, sends the delegate object a tableView(_:accessoryButtonTappedForRowWith:) message.

The accessory type cross-fades between normal and editing states if it set for both states; use the accessoryType property to set the accessory view for the cell during the table view’s normal state. If this property is not set for both states, the cell is animated to slide or out, as necessary.

## See Also

### Related Documentation

func willTransition(to: UITableViewCell.StateMask)

Notifies the cell that it’s about to transition to a new cell state.

func didTransition(to: UITableViewCell.StateMask)

Notifies the cell that it transitioned to a new cell state.

### Managing accessory views

var accessoryType: UITableViewCell.AccessoryType

The type of standard accessory view for the cell to use in the table view’s normal state.

var accessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s normal state.

var editingAccessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s editing state.

enum AccessoryType

The type of standard accessory control used by a cell.

