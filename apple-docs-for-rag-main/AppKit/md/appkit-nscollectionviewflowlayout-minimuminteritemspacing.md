

- AppKit
- NSCollectionViewFlowLayout
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

If the delegate does not implement the collectionView(_:layout:minimumInteritemSpacingForSectionAt:) method, the flow layout object uses the value of this property to set the spacing between items in the same line.

For a vertically scrolling layout, the value represents the minimum spacing between items in the same row. For a horizontally scrolling layout, the value represents the minimum spacing between items in the same column. The layout object uses this spacing only to compute how many items can fit in a single row or column. The actual spacing may be increased after the number of items has been determined, as illustrated in Figure 1.

The default value of this property is `10.0`.

## See Also

### Configuring the Item Spacing

var minimumLineSpacing: CGFloat

The minimum spacing (in points) to use between rows or columns.

var estimatedItemSize: NSSize

The estimated size of items in the collection view.

var itemSize: NSSize

The default size to use for items.

var sectionInset: NSEdgeInsets

The margins used to lay out content in a section.

