

- UIKit
- UICollectionViewFlowLayout
-  estimatedItemSize 

Instance Property

# estimatedItemSize

The estimated size of cells in the collection view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var estimatedItemSize: CGSize { get set }
```

## Discussion

Providing an estimated cell size can improve the performance of the collection view when the cells adjust their size dynamically. The estimated value lets the collection view defer some calculations to determine the actual size of its content. Cells that aren’t onscreen are assumed to be the estimated height.

The default value of this property is CGSizeZero. Setting it to any other value, like automaticSize, causes the collection view to query each cell for its actual size using the cell’s preferredLayoutAttributesFitting(_:) method.

If all of your cells are the same size, use the itemSize property, instead of this property, to specify the cell size instead.

## See Also

### Configuring item spacing

var minimumLineSpacing: CGFloat

The minimum spacing to use between lines of items in the grid.

var minimumInteritemSpacing: CGFloat

The minimum spacing to use between items in the same row.

var itemSize: CGSize

The default size to use for cells.

class let automaticSize: CGSize

A placeholder size for self-sizing cells.

var sectionInset: UIEdgeInsets

The margins used to lay out content in a section.

var sectionInsetReference: UICollectionViewFlowLayout.SectionInsetReference

The boundary that section insets are defined in relation to.

enum SectionInsetReference

Constants that describe the reference point of the section insets.

