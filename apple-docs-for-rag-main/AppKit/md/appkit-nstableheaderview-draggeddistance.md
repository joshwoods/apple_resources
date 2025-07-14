

- AppKit
- NSTableHeaderView
-  draggedDistance 

Instance Property

# draggedDistance

The horizontal distance that the user has dragged a column.

macOS

``` source
@MainActor
var draggedDistance: CGFloat { get }
```

## Discussion

If the user is dragging a column, this property contains that column’s horizontal distance from its original position; otherwise, the property’s value is undefined.

## See Also

### Checking altered columns

var draggedColumn: Int

The index of the column that the user is dragging.

var resizedColumn: Int

The index of the column that the user is resizing.

