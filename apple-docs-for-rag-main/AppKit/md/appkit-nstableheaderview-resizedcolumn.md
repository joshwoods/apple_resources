

- AppKit
- NSTableHeaderView
-  resizedColumn 

Instance Property

# resizedColumn

The index of the column that the user is resizing.

macOS

``` source
@MainActor
var resizedColumn: Int { get }
```

## Discussion

If the user is resizing a column, this property contains the index of that column; otherwise, it contains `-1`.

## See Also

### Checking altered columns

var draggedColumn: Int

The index of the column that the user is dragging.

var draggedDistance: CGFloat

The horizontal distance that the user has dragged a column.

