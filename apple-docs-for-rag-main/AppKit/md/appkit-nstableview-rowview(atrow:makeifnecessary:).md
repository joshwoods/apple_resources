

- AppKit
- NSTableView
-  rowView(atRow:makeIfNecessary:) 

Instance Method

# rowView(atRow:makeIfNecessary:)

Returns a row view at the specified index, creating one if necessary.

macOS 10.7+

``` source
@MainActor
func rowView(
    atRow row: Int,
    makeIfNecessary: Bool
) -> NSTableRowView?
```

## Parameters 

`row`  

The row index.

`makeIfNecessary`  

true if a view is required, false if you want to update properties on a view, if one is available.

## Return Value

An instance, or subclass, of NSTableRowView. Returning `nil` is also valid if `makeIfNecessary` is false and the view did not exist.

## Discussion

This method first attempts to return a currently displayed view in the visible area. If there is no visible view, and `makeIfNecessary` is true, a prepared temporary view is returned. If `makeIfNecessary` is false, and the view is not visible, `nil` is returned.

In general, `makeIfNecessary` should be true if you require a resulting view, and false if you want to update properties on a view only if it is available (generally this means it is visible).

An exception is thrown if `row` falls outside of the number of rows in the table (numberOfRows). The returned result should generally not be held onto for longer than the current run loop cycle. It’s better to call rowView(atRow:makeIfNecessary:) whenever a view is required.

## See Also

### Creating Views to Display

func makeView(withIdentifier: NSUserInterfaceItemIdentifier, owner: Any?) -> NSView?

Returns a new or existing view with the specified identifier.

func view(atColumn: Int, row: Int, makeIfNecessary: Bool) -> NSView?

Returns a view at the specified row and column indexes, creating one if necessary.

struct NSUserInterfaceItemIdentifier

