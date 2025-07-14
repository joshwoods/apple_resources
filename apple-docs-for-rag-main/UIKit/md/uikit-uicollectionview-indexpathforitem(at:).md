

- UIKit
- UICollectionView
-  indexPathForItem(at:) 

Instance Method

# indexPathForItem(at:)

Gets the index path of the item at the specified point in the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func indexPathForItem(at point: CGPoint) -> IndexPath?
```

## Parameters 

`point`  

A point in the collection view’s coordinate system.

## Return Value

The index path of the item at the specified point or `nil` if no item was found at the specified point.

## Discussion

This method relies on the layout information provided by the associated layout object to determine which item contains the point.

## See Also

### Locating items and views in the collection view

var indexPathsForVisibleItems: [IndexPath]

An array of the visible items in the collection view.

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

