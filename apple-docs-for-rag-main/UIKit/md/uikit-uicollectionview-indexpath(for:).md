

- UIKit
- UICollectionView
-  indexPath(for:) 

Instance Method

# indexPath(for:)

Gets the index path of the specified cell.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func indexPath(for cell: UICollectionViewCell) -> IndexPath?
```

## Parameters 

`cell`  

The cell object whose index path you want.

## Return Value

The index path of the cell or `nil` if the specified cell is not in the collection view.

## See Also

### Locating items and views in the collection view

func indexPathForItem(at: CGPoint) -> IndexPath?

Gets the index path of the item at the specified point in the collection view.

var indexPathsForVisibleItems: [IndexPath]

An array of the visible items in the collection view.

func cellForItem(at: IndexPath) -> UICollectionViewCell?

Gets the cell object at the index path you specify.

func indexPathsForVisibleSupplementaryElements(ofKind: String) -> [IndexPath]

Gets the index paths of all visible supplementary views of the specified type.

func supplementaryView(forElementKind: String, at: IndexPath) -> UICollectionReusableView?

Gets the supplementary view at the specified index path.

func visibleSupplementaryViews(ofKind: String) -> [UICollectionReusableView]

Gets an array of the visible supplementary views of the specified kind.

