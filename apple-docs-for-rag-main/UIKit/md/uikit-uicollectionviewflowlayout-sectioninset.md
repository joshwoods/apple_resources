

- UIKit
- UICollectionViewFlowLayout
-  sectionInset 

Instance Property

# sectionInset

The margins used to lay out content in a section.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var sectionInset: UIEdgeInsets { get set }
```

## Discussion

If the delegate object does not implement the collectionView(_:layout:insetForSectionAt:) method, the flow layout uses the value in this property to set the margins for each section.

Section insets reflect the spacing at the outer edges of the section. The margins affect the initial position of the header view, the minimum space on either side of each line of items, and the distance from the last line to the footer view. The margin insets do not affect the size of the header and footer views in the non scrolling direction.

The default edge insets are all set to `0`.

## See Also

### Configuring item spacing

var minimumLineSpacing: CGFloat

The minimum spacing to use between lines of items in the grid.

var minimumInteritemSpacing: CGFloat

The minimum spacing to use between items in the same row.

var itemSize: CGSize

The default size to use for cells.

var estimatedItemSize: CGSize

The estimated size of cells in the collection view.

class let automaticSize: CGSize

A placeholder size for self-sizing cells.

var sectionInsetReference: UICollectionViewFlowLayout.SectionInsetReference

The boundary that section insets are defined in relation to.

enum SectionInsetReference

Constants that describe the reference point of the section insets.

