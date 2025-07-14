

- UIKit
- UICollectionViewFlowLayout
-  sectionInsetReference 

Instance Property

# sectionInsetReference

The boundary that section insets are defined in relation to.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var sectionInsetReference: UICollectionViewFlowLayout.SectionInsetReference { get set }
```

## Discussion

The default value of this property is UICollectionViewFlowLayout.SectionInsetReference.fromContentInset.

The minimum value of this property is always the collection view’s contentInset. For example, if the value of this property is UICollectionViewFlowLayout.SectionInsetReference.fromSafeArea, but the adjusted content inset is greater than the combination of the safe area and section insets, then the section’s content is aligned with the content inset instead.

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

var sectionInset: UIEdgeInsets

The margins used to lay out content in a section.

enum SectionInsetReference

Constants that describe the reference point of the section insets.

