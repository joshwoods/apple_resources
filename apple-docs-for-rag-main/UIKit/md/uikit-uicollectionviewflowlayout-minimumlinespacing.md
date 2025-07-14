

- UIKit
- UICollectionViewFlowLayout
-  minimumLineSpacing 

Instance Property

# minimumLineSpacing

The minimum spacing to use between lines of items in the grid.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var minimumLineSpacing: CGFloat { get set }
```

## Discussion

If the delegate object does not implement the collectionView(_:layout:minimumLineSpacingForSectionAt:) method, the flow layout uses the value in this property to set the spacing between lines in a section.

For a vertically scrolling grid, this value represents the minimum spacing between successive rows. For a horizontally scrolling grid, this value represents the minimum spacing between successive columns. This spacing is not applied to the space between the header and the first line or between the last line and the footer.

The default value of this property is 10.0.

## See Also

### Configuring item spacing

var minimumInteritemSpacing: CGFloat

The minimum spacing to use between items in the same row.

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

