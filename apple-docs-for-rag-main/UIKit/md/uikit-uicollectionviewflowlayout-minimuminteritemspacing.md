

- UIKit
- UICollectionViewFlowLayout
-  minimumInteritemSpacing 

Instance Property

# minimumInteritemSpacing

The minimum spacing to use between items in the same row.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var minimumInteritemSpacing: CGFloat { get set }
```

## Discussion

If the delegate object does not implement the collectionView(_:layout:minimumInteritemSpacingForSectionAt:) method, the flow layout uses the value in this property to set the spacing between items in the same line.

For a vertically scrolling grid, this value represents the minimum spacing between items in the same row. For a horizontally scrolling grid, this value represents the minimum spacing between items in the same column. This spacing is used to compute how many items can fit in a single line, but after the number of items is determined, the actual spacing may possibly be adjusted upward.

The default value of this property is 10.0.

## See Also

### Configuring item spacing

var minimumLineSpacing: CGFloat

The minimum spacing to use between lines of items in the grid.

var itemSize: CGSize

The default size to use for cells.

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

