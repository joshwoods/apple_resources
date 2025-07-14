

- AppKit
- NSTableHeaderView
-  draggedColumn 

Instance Property

# draggedColumn

The index of the column that the user is dragging.

macOS

``` source
@MainActor
var draggedColumn: Int { get }
```

## Discussion

If the user is dragging a column, this property contains the index of that column; otherwise, it contains `-1`.

## See Also

### Checking altered columns

var draggedDistance: CGFloat

The horizontal distance that the user has dragged a column.

var resizedColumn: Int

The index of the column that the user is resizing.

