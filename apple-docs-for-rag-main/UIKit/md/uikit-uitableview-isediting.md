

- UIKit
- UITableView
-  isEditing 

Instance Property

# isEditing

A Boolean value that determines whether the table view is in editing mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isEditing: Bool { get set }
```

## Discussion

When the value of this property is true, the table view is in editing mode: The cells of the table might show an insertion or deletion control on the left side of each cell and a reordering control on the right side, depending on how the cell is configured. (See UITableViewCell for details.) Tapping a control causes the table view to invoke the data source method tableView(_:commit:forRowAt:). The default value is false.

## See Also

### Putting the table into edit mode

func setEditing(Bool, animated: Bool)

Toggles the table view into and out of editing mode.

