

- AppKit
- NSCollectionViewFlowLayout
-  sectionInset 

Instance Property

# sectionInset

The margins used to lay out content in a section.

macOS 10.11+

``` source
@MainActor
var sectionInset: NSEdgeInsets { get set }
```

## Discussion

If the delegate does not implement the collectionView(_:layout:insetForSectionAt:) method, the flow layout object uses the value of this property to set the margins for each section.

Section insets reflect the spacing at the outer edges of the section. The margins affect the positioning of the header view, the minimum space on either side of each line of items, and the distance from the last line to the footer view, as shown in Figure 1. The margin insets do not affect the size of the header and footer views in the nonscrolling direction.

The default insets are all set to `0`.

## See Also

### Configuring the Item Spacing

var minimumLineSpacing: CGFloat

The minimum spacing (in points) to use between rows or columns.

var minimumInteritemSpacing: CGFloat

The minimum spacing (in points) to use between items in the same row or column.

var estimatedItemSize: NSSize

The estimated size of items in the collection view.

var itemSize: NSSize

The default size to use for items.

