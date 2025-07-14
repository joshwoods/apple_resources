

- AppKit
- NSTableView
-  usesStaticContents 

Instance Property

# usesStaticContents

A Boolean value indicating whether the table uses static data.

macOS 10.10+

``` source
@MainActor
var usesStaticContents: Bool { get set }
```

## Discussion

A static table does not rely on a data source to provide the number of rows. A static table view’s contents are set at design time and can be changed programmatically as needed. Typically, you do not change the contents of a static table view after setting them.

In Xcode, any rows you add to a static table are saved in the corresponding nib or storyboard file and loaded with the rest of the table at runtime. You can add table rows programmatically to a static table view using the insertRows(at:withAnimation:) method. When adding rows programmatically, your table view delegate must implement the tableView(_:viewFor:row:) method to provide the corresponding view for any new rows. You can also remove rows at any time using the removeRows(at:withAnimation:) method.

Note

A table with static contents must be an NSView-based table view.

## See Also

### Managing the Table’s Data

var dataSource: (any NSTableViewDataSource)?

The object that provides the data displayed by the table view.

func reloadData()

Marks the table view as needing redisplay, so it will reload the data for visible cells and draw the new values.

func reloadData(forRowIndexes: IndexSet, columnIndexes: IndexSet)

Reloads the data for only the specified rows and columns.

