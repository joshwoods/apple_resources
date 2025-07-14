

- UIKit
- UICollectionViewFlowLayout
-  UICollectionViewFlowLayout.SectionInsetReference 

Enumeration

# UICollectionViewFlowLayout.SectionInsetReference

Constants that describe the reference point of the section insets.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
enum SectionInsetReference
```

## Topics

### Constants

case fromContentInset

Section insets are defined in relation to the collection view’s content inset.

case fromLayoutMargins

Section insets are defined in relation to the margins of the layout.

case fromSafeArea

Section insets are defined in relation to the safe area of the layout.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var sectionInsetReference: UICollectionViewFlowLayout.SectionInsetReference

The boundary that section insets are defined in relation to.

