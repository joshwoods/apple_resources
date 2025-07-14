

- UIKit
- UICollectionView
-  indexPathsForVisibleItems 

Instance Property

# indexPathsForVisibleItems

An array of the visible items in the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var indexPathsForVisibleItems: [IndexPath] { get }
```

## Discussion

The value of this property is an unsorted array of NSIndexPath objects, each of which corresponds to a visible cell in the collection view. This array doesn’t include any supplementary views that are currently visible. If there are no visible items, the value of this property is an empty array.

## See Also

### Related Documentation

var visibleCells: [UICollectionViewCell]

An array of visible cells currently displayed by the collection view.

### Locating items and views in the collection view

func indexPathForItem(at: CGPoint) -> IndexPath?

Gets the index path of the item at the specified point in the collection view.

func indexPath(for: UICollectionViewCell) -> IndexPath?

Gets the index path of the specified cell.

func cellForItem(at: IndexPath) -> UICollectionViewCell?

Gets the cell object at the index path you specify.

func indexPathsForVisibleSupplementaryElements(ofKind: String) -> [IndexPath]

Gets the index paths of all visible supplementary views of the specified type.

func supplementaryView(forElementKind: String, at: IndexPath) -> UICollectionReusableView?

Gets the supplementary view at the specified index path.

func visibleSupplementaryViews(ofKind: String) -> [UICollectionReusableView]

Gets an array of the visible supplementary views of the specified kind.

