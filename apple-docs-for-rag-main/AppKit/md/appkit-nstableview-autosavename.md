

- AppKit
- NSTableView
-  autosaveName 

Instance Property

# autosaveName

The name under which table information is automatically saved.

macOS

``` source
@MainActor
var autosaveName: NSTableView.AutosaveName? { get set }
```

## Discussion

The table information is saved separately in user defaults for each user and for each application that user uses. If no name has been set, the value of this property is `nil`. Even when a table view has an autosave name, it only saves the table information when the autosaveTableColumns property is true.

If you change the value of this property to a new name, the table reads in any saved information and sets the order and width of this table view’s columns to match. Setting the name to `nil` removes any previously stored state from the user defaults.

## See Also

### Table Column State Persistence

var autosaveTableColumns: Bool

A Boolean value indicating whether the order and width of the table view’s columns are automatically saved.

typealias AutosaveName

