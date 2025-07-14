

- UIKit
- UICollectionViewFlowLayout
-  itemSize 

Instance Property

# itemSize

The default size to use for cells.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var itemSize: CGSize { get set }
```

## Discussion

If the delegate does not implement the collectionView(_:layout:sizeForItemAt:) method, the flow layout uses the value in this property to set the size of each cell. This results in cells that all have the same size.

The default size value is (50.0, 50.0).

## See Also

### Configuring item spacing

var minimumLineSpacing: CGFloat

The minimum spacing to use between lines of items in the grid.

var minimumInteritemSpacing: CGFloat

The minimum spacing to use between items in the same row.

var estimatedItemSize: CGSize

The estimated size of cells in the collection view.

class let automaticSize: CGSize

A placeholder size for self-sizing cells.

var sectionInset: UIEdgeInsets

The margins used to lay out content in a section.

var sectionInsetReference: UICollectionViewFlowLayout.SectionInsetReference

The boundary that section insets are defined in relation to.

enum SectionInsetReference

Constants that describe the reference point of the section insets.

