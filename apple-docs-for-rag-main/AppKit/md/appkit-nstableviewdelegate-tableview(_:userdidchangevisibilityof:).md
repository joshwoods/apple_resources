

- AppKit
- NSTableViewDelegate
-  tableView(\_:userDidChangeVisibilityOf:) 

Instance Method

# tableView(\_:userDidChangeVisibilityOf:)

Tells the delegate that the user changed the visibility of one or more table columns.

macOS 14.0+

``` source
optional func tableView(
    _ tableView: NSTableView,
    userDidChangeVisibilityOf columns: [NSTableColumn]
)
```

## Parameters 

`tableView`  

The table view object requesting this information.

`columns`  

The table columns affected by the visibility change.

## See Also

### Showing and hiding columns

func tableView(NSTableView, userCanChangeVisibilityOf: NSTableColumn) -> Bool

Asks the delegate to verify that the user can change the given column’s visibility.

