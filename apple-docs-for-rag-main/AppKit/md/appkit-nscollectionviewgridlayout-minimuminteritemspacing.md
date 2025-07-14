

- AppKit
- NSCollectionViewGridLayout
-  minimumInteritemSpacing 

Instance Property

# minimumInteritemSpacing

The minimum spacing (in points) to use between items in the same row or column.

macOS 10.11+

``` source
@MainActor
var minimumInteritemSpacing: CGFloat { get set }
```

## Discussion

For a vertically scrolling layout, the value represents the minimum spacing between items in the same row. For a horizontally scrolling layout, the value represents the minimum spacing between items in the same column. The layout object uses this spacing only to compute how many items can fit in a single row or column. The actual spacing may be increased after the number of items has been determined.

The default value of this property is `0.0`.

## See Also

### Specifying the Grid Layout Attributes

var minimumLineSpacing: CGFloat

The minimum spacing (in points) to use between rows or columns.

var margins: NSEdgeInsets

The amount of empty space (in points) around the grid’s content.

