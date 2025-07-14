

- AppKit
- NSTableView
-  enumerateAvailableRowViews(\_:) 

Instance Method

# enumerateAvailableRowViews(\_:)

Allows the enumeration of all the table rows that are known to the table view.

macOS 10.7+

``` source
@MainActor
func enumerateAvailableRowViews(_ handler: (NSTableRowView, Int) -> Void)
```

## Parameters 

`handler`  

The `Block` to apply to elements in the set.

The `Block` takes two arguments:

rowView  
The view for the row.

row  
The index of the row.

## Discussion

The enumeration includes all views in the visibleRect; however, it may also include ones that are “in flight” due to animations or other attributes of the table.

It is preferred to use this method to efficiently make changes over all views that exist in the table.

Note

There is no guarantee that the rows will be enumerated in the displayed order.

