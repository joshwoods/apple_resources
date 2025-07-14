

- UIKit
- UITableViewCell
-  didTransition(to:) 

Instance Method

# didTransition(to:)

Notifies the cell that it transitioned to a new cell state.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func didTransition(to state: UITableViewCell.StateMask)
```

## Parameters 

`state`  

A bit mask indicating the state or combination of states the cell is transitioning to.

## Discussion

Subclasses of `UITableViewCell` can implement this method to animate additional changes to a cell when it is changing state. `UITableViewCell` calls this method whenever a cell transitions between states, such as from a normal state (the default) to editing mode. This method is called at the end of the animation block, which gives the custom cell a chance to clean up after the state change—for example, removing the edit and reorder controls after transitioning out of editing. Subclasses must always call `super` when overriding this method.

Note that when the user swipes a cell to delete it, the cell transitions to the state identified by the showingDeleteConfirmation constant but the showingEditControl is not set.

## See Also

### Related Documentation

var editingAccessoryType: UITableViewCell.AccessoryType

The type of standard accessory view for the cell to use in the table view’s editing state.

var editingAccessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s editing state.

var accessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s normal state.

var accessoryType: UITableViewCell.AccessoryType

The type of standard accessory view for the cell to use in the table view’s normal state.

### Adjusting to state transitions

func willTransition(to: UITableViewCell.StateMask)

Notifies the cell that it’s about to transition to a new cell state.

struct StateMask

Constants used to determine the new state of a cell as it transitions between states.

