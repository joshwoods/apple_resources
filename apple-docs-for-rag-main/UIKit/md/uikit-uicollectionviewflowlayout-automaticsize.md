

- UIKit
- UICollectionViewFlowLayout
-  automaticSize 

Type Property

# automaticSize

A placeholder size for self-sizing cells.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class let automaticSize: CGSize
```

## Discussion

Set this constant as the value for the estimatedItemSize property to enable self-sizing cells for your collection view. This is a non-zero, placeholder value that tells the collection view to query each cell for its actual size using the cell’s preferredLayoutAttributesFitting(_:) method.

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

var sectionInset: UIEdgeInsets

The margins used to lay out content in a section.

var sectionInsetReference: UICollectionViewFlowLayout.SectionInsetReference

The boundary that section insets are defined in relation to.

enum SectionInsetReference

Constants that describe the reference point of the section insets.

