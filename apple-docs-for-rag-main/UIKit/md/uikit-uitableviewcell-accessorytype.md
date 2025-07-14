

- UIKit
- UITableViewCell
-  accessoryType 

Instance Property

# accessoryType

The type of standard accessory view for the cell to use in the table view’s normal state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var accessoryType: UITableViewCell.AccessoryType { get set }
```

## Mentioned in 

Handling row selection in a table view

Configuring the cells for your table

## Discussion

The accessory view appears in the right side of the cell in the table view’s normal (default) state. The standard accessory views include the disclosure chevron; for a description of valid accessoryType constants, see UITableViewCell.AccessoryType. The default is UITableViewCell.AccessoryType.none. If a custom accessory view is set through the accessoryView property, the value of this property is ignored. If the cell is enabled and the accessory type is UITableViewCell.AccessoryType.detailDisclosureButton, the accessory view tracks touches and, when tapped, sends the data-source object a tableView(_:accessoryButtonTappedForRowWith:) message.

The accessory-type image cross-fades between normal and editing states if it set for both states; use the editingAccessoryType property to set the accessory type for the cell during editing mode. If this property is not set for both states, the cell is animated to slide in or out, as necessary.

## See Also

### Related Documentation

func willTransition(to: UITableViewCell.StateMask)

Notifies the cell that it’s about to transition to a new cell state.

func didTransition(to: UITableViewCell.StateMask)

Notifies the cell that it transitioned to a new cell state.

### Managing accessory views

var accessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s normal state.

var editingAccessoryType: UITableViewCell.AccessoryType

The type of standard accessory view for the cell to use in the table view’s editing state.

var editingAccessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s editing state.

enum AccessoryType

The type of standard accessory control used by a cell.

