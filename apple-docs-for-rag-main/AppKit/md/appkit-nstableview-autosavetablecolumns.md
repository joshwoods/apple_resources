

- AppKit
- NSTableView
-  autosaveTableColumns 

Instance Property

# autosaveTableColumns

A Boolean value indicating whether the order and width of the table view’s columns are automatically saved.

macOS

``` source
@MainActor
var autosaveTableColumns: Bool { get set }
```

## Discussion

When this property is set to true, the table information is saved separately for each user and application under the name specified in the autosaveName property. If you change the value of this property from false to true, the table tries to read in any saved information and sets the order and width of this table view’s columns to match. If the autosaveName property is `nil`, this setting is ignored and the table information is not read or saved.

When autosave is enabled, the table saves the table column width, the table column order, any applied sort descriptors, and the table column hidden state (in macOS 10.5 and later).

## See Also

### Table Column State Persistence

var autosaveName: NSTableView.AutosaveName?

The name under which table information is automatically saved.

typealias AutosaveName

