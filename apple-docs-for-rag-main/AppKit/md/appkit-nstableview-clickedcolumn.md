

- AppKit
- NSTableView
-  clickedColumn 

Instance Property

# clickedColumn

The index of the column the user clicked.

macOS

``` source
@MainActor
var clickedColumn: Int { get }
```

## Discussion

This property contains the index in the tableColumns array of the column that the user clicked. The value is `-1` when the user clicks in an area of the table view that is not occupied by columns or when the user clicks a row that is a group separator.

The value of this property is meaningful in the target object’s implementation of the action and double-action methods. You can also use the value to determine which contextual menu to display when the user Control-clicks in a table. Note that the `clickedColumn` value remains valid when the menu item sends the action message. To see an example of using `clickedColumn` in the implementation of a contextual menu, download the DragNDropOutlineView: implementing drag and drop in an NSOutlineView sample project.

## See Also

### Related Documentation

var action: Selector?

The default action-message selector associated with the control.

### Target-action Behavior

var doubleAction: Selector?

The message sent to the table view’s target when the user double-clicks a cell or column header.

var clickedRow: Int

The index of the row the user clicked.

