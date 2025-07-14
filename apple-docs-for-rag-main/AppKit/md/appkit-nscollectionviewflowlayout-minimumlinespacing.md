

- AppKit
- NSCollectionViewFlowLayout
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

If the delegate does not implement the collectionView(_:layout:minimumLineSpacingForSectionAt:) method, the flow layout object uses the value of this property to set the spacing between rows or columns.

For a vertically scrolling layout, the value represents the minimum spacing between successive rows. For a horizontally scrolling layout, the value represents the minimum spacing between successive columns. This spacing is not applied to the space between the header view and the first line or between the last line and the footer view. Figure 1 shows how the line spacing is applied to rows of unevenly sized items, illustrating how the actual spacing between individual items may be greater than the minimum value.

The default value of this property is `10.0`.

## See Also

### Configuring the Item Spacing

var minimumInteritemSpacing: CGFloat

The minimum spacing (in points) to use between items in the same row or column.

var estimatedItemSize: NSSize

The estimated size of items in the collection view.

var itemSize: NSSize

The default size to use for items.

var sectionInset: NSEdgeInsets

The margins used to lay out content in a section.

