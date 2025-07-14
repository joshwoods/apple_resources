

- AppKit
- NSCollectionViewGridLayout
-  minimumLineSpacing 

Instance Property

# minimumLineSpacing

The minimum spacing (in points) to use between rows or columns.

macOS 10.11+

``` source
@MainActor
var minimumLineSpacing: CGFloat { get set }
```

## Discussion

For a vertically scrolling layout, the value represents the minimum spacing between successive rows. For a horizontally scrolling layout, the value represents the minimum spacing between successive columns. This spacing is not applied to the space between the header view and the first line or between the last line and the footer view.

The default value of this property is `0.0`.

## See Also

### Specifying the Grid Layout Attributes

var minimumInteritemSpacing: CGFloat

The minimum spacing (in points) to use between items in the same row or column.

var margins: NSEdgeInsets

The amount of empty space (in points) around the grid’s content.

