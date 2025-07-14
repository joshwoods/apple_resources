

- AppKit
- NSTableView
-  didAdd(\_:forRow:) 

Instance Method

# didAdd(\_:forRow:)

Invoked when a row view is added to the table.

macOS 10.7+

``` source
@MainActor
func didAdd(
    _ rowView: NSTableRowView,
    forRow row: Int
)
```

## Parameters 

`rowView`  

The row view.

`row`  

The row index.

## Discussion

The subclass can implement this method to be alerted when `rowView` has been added to the table. At this point, the subclass can choose to add in extra views, or modify any properties of `rowView`. Subclasses must be sure to call super.

Note

This method is only applicable to NSView-based table views.

## See Also

### Adding and Deleting Row Views

func didRemove(NSTableRowView, forRow: Int)

Invoked when a row view is removed from the table.

