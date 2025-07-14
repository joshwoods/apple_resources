

- AppKit
- NSCollectionViewFlowLayout
-  estimatedItemSize 

Instance Property

# estimatedItemSize

The estimated size of items in the collection view.

macOS 10.11+

``` source
@MainActor
var estimatedItemSize: NSSize { get set }
```

## Discussion

Providing an estimated item size lets the collection view defer some of the calculations needed to determine the size of its content, which can improve performance. Instead of explicitly computing the size of each item, the flow layout assumes that offscreen items have the estimated size. The estimated size is used only until an actual value is calculated. The default value of this property is NSZeroSize.

If the value of this property is not NSZeroSize, the flow layout uses the estimated size you specified. If all of your items actually have the same size, use the itemSize property to set their size and set this property to NSZeroSize. For more information about how item sizes are determined, see Understanding How the Flow Layout is Generated.

## See Also

### Configuring the Item Spacing

var minimumLineSpacing: CGFloat

The minimum spacing (in points) to use between rows or columns.

var minimumInteritemSpacing: CGFloat

The minimum spacing (in points) to use between items in the same row or column.

var itemSize: NSSize

The default size to use for items.

var sectionInset: NSEdgeInsets

The margins used to lay out content in a section.

