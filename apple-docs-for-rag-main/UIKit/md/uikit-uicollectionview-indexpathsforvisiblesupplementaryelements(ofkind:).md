

- UIKit
- UICollectionView
-  indexPathsForVisibleSupplementaryElements(ofKind:) 

Instance Method

# indexPathsForVisibleSupplementaryElements(ofKind:)

Gets the index paths of all visible supplementary views of the specified type.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func indexPathsForVisibleSupplementaryElements(ofKind elementKind: String) -> [IndexPath]
```

## Parameters 

`elementKind`  

The kind of supplementary view to locate. This value is defined by the layout object. This parameter must not be `nil`.

## Return Value

An array of NSIndexPath objects, each of which corresponds to a visible supplementary view in the collection view. If there are no visible supplementary views, this method returns an empty array.

## See Also

### Locating items and views in the collection view

func indexPathForItem(at: CGPoint) -> IndexPath?

Gets the index path of the item at the specified point in the collection view.

var indexPathsForVisibleItems: [IndexPath]

An array of the visible items in the collection view.

func indexPath(for: UICollectionViewCell) -> IndexPath?

Gets the index path of the specified cell.

func cellForItem(at: IndexPath) -> UICollectionViewCell?

Gets the cell object at the index path you specify.

func supplementaryView(forElementKind: String, at: IndexPath) -> UICollectionReusableView?

Gets the supplementary view at the specified index path.

func visibleSupplementaryViews(ofKind: String) -> [UICollectionReusableView]

Gets an array of the visible supplementary views of the specified kind.

