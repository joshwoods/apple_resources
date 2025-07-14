

- UIKit
- UICollectionView
-  visibleSupplementaryViews(ofKind:) 

Instance Method

# visibleSupplementaryViews(ofKind:)

Gets an array of the visible supplementary views of the specified kind.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func visibleSupplementaryViews(ofKind elementKind: String) -> [UICollectionReusableView]
```

## Parameters 

`elementKind`  

The kind of supplementary view to locate. This value is defined by the layout object. This parameter must not be `nil`.

## Return Value

An array of the visible supplementary views. If no supplementary views are visible, the returned array is empty.

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

func indexPathsForVisibleSupplementaryElements(ofKind: String) -> [IndexPath]

Gets the index paths of all visible supplementary views of the specified type.

func supplementaryView(forElementKind: String, at: IndexPath) -> UICollectionReusableView?

Gets the supplementary view at the specified index path.

