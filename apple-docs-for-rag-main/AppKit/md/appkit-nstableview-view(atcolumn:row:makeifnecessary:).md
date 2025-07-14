

- AppKit
- NSTableView
-  view(atColumn:row:makeIfNecessary:) 

Instance Method

# view(atColumn:row:makeIfNecessary:)

Returns a view at the specified row and column indexes, creating one if necessary.

macOS 10.7+

``` source
@MainActor
func view(
    atColumn column: Int,
    row: Int,
    makeIfNecessary: Bool
) -> NSView?
```

## Parameters 

`column`  

The index of the column in the tableColumns array.

`row`  

The row index.

`makeIfNecessary`  

true if a view is required, false if you want to update properties on a view, if one is available.

## Return Value

An instance of NSView.

## Discussion

This method first attempts to return an available view, which is generally in the visible area. If there is no available view, and `makeIfNecessary` is true, a prepared temporary view is returned. If `makeIfNecessary` is false, and the view is not available, `nil` will be returned.

In general, `makeIfNecessary` should be true if you require a resulting view, and false if you only want to update properties on a view only if it is available (generally this means it is visible).

An exception will be thrown if `row` is not within the numberOfRows. The returned result should generally not be held onto for longer than the current run loop cycle. Instead they should re-query the table view for the row view.

## See Also

### Creating Views to Display

func makeView(withIdentifier: NSUserInterfaceItemIdentifier, owner: Any?) -> NSView?

Returns a new or existing view with the specified identifier.

func rowView(atRow: Int, makeIfNecessary: Bool) -> NSTableRowView?

Returns a row view at the specified index, creating one if necessary.

struct NSUserInterfaceItemIdentifier

