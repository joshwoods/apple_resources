

- UIKit
- UITableView
-  setEditing(\_:animated:) 

Instance Method

# setEditing(\_:animated:)

Toggles the table view into and out of editing mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setEditing(
    _ editing: Bool,
    animated: Bool
)
```

## Parameters 

`editing`  

true to enter editing mode; false to leave it. The default value is false.

`animated`  

true to animate the transition to editing mode; false to make the transition immediate.

## Discussion

When you call this method with the value of `editing` set to true, the table view goes into editing mode by calling setEditing(_:animated:) on each visible `UITableViewCell` object. Calling this method with `editing` set to false turns off editing mode. In editing mode, the cells of the table might show an insertion or deletion control on the left side of each cell and a reordering control on the right side, depending on how the cell is configured. (See UITableViewCell for details.) The data source of the table view can selectively exclude cells from editing mode by implementing tableView(_:canEditRowAt:).

## See Also

### Putting the table into edit mode

var isEditing: Bool

A Boolean value that determines whether the table view is in editing mode.

