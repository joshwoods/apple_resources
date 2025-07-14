

- AppKit
- NSCollectionViewFlowLayout
-  itemSize 

Instance Property

# itemSize

The default size to use for items.

macOS 10.11+

``` source
@MainActor
var itemSize: NSSize { get set }
```

## Discussion

This property contains the default size of items. If you do not provide an estimated size or implement the collectionView(_:layout:sizeForItemAt:) method in your delegate, the flow layout uses this value for the size of each item. All items are set to the same size. This value applies only to items and not to supplementary views.

The default value of this property is (`50.0`, `50.0`). For more information about how item sizes are determined, see Understanding How the Flow Layout is Generated.

## See Also

### Configuring the Item Spacing

var minimumLineSpacing: CGFloat

The minimum spacing (in points) to use between rows or columns.

var minimumInteritemSpacing: CGFloat

The minimum spacing (in points) to use between items in the same row or column.

var estimatedItemSize: NSSize

The estimated size of items in the collection view.

var sectionInset: NSEdgeInsets

The margins used to lay out content in a section.

