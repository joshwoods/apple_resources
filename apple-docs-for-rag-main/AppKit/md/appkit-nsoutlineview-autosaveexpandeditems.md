

- AppKit
- NSOutlineView
-  autosaveExpandedItems 

Instance Property

# autosaveExpandedItems

A Boolean value indicating whether the expanded items are automatically saved across launches of the app.

macOS

``` source
@MainActor
var autosaveExpandedItems: Bool { get set }
```

## Discussion

When the value of this property is true, the outline view saves the state of its expanded items and restores that state the next time the user launches the app. (If the outline view’s autosaveName property is `nil`, or if you have not implemented the outlineView(_:itemForPersistentObject:) and outlineView(_:persistentObjectForItem:) delegate methods, this setting is ignored and outline information is not saved.) The configuration data is saved separately for each user and for each app. The default value of this property is false.

You can have separate settings for the autosaveExpandedItems and autosaveTableColumns properties, so you could, for example, save expanded item information, but not table column positions.

## See Also

### Related Documentation

var autosaveTableColumns: Bool

A Boolean value indicating whether the order and width of the table view’s columns are automatically saved.

var autosaveName: NSTableView.AutosaveName?

The name under which table information is automatically saved.

