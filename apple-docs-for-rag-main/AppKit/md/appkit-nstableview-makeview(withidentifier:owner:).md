

- AppKit
- NSTableView
-  makeView(withIdentifier:owner:) 

Instance Method

# makeView(withIdentifier:owner:)

Returns a new or existing view with the specified identifier.

macOS 10.7+

``` source
@MainActor
func makeView(
    withIdentifier identifier: NSUserInterfaceItemIdentifier,
    owner: Any?
) -> NSView?
```

## Parameters 

`identifier`  

The view identifier. Must not be `nil`.

`owner`  

The owner of the NIB that may be loaded and instantiated to create a new view with the specified identifier.

## Return Value

A view for the row.

## Discussion

Typically, `identifier` is associated with a cell view that’s contained in a table’s Nib file. When this method is called, the table view automatically instantiates the cell view with the specified owner, which is usually the table view’s delegate. (The owner is useful in setting up outlets and target/actions from the view.) Note that a cell view’s identifier must be the same as its table column’s identifier for bindings to work. If you’re using bindings, it’s recommended that you use the Automatic identifier setting in Interface Builder.

This method may also return a reused view with the same `identifier` that is no longer available on screen. If a view with the specified identifier can’t be instantiated from the nib file or found in the reuse queue, this method returns `nil`.

This method is usually called by the delegate in tableView(_:viewFor:row:), but it can also be overridden to provide custom views for the `identifier`. Note that awakeFromNib() is called each time this method is called, which means that `awakeFromNib` is also called on `owner`, even though the owner is already awake.

## See Also

### Related Documentation

Table View Programming Guide for Mac

Drag and Drop Programming Topics

### Creating Views to Display

func rowView(atRow: Int, makeIfNecessary: Bool) -> NSTableRowView?

Returns a row view at the specified index, creating one if necessary.

func view(atColumn: Int, row: Int, makeIfNecessary: Bool) -> NSView?

Returns a view at the specified row and column indexes, creating one if necessary.

struct NSUserInterfaceItemIdentifier

