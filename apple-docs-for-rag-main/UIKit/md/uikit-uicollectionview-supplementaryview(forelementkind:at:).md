

- UIKit
- UICollectionView
-  supplementaryView(forElementKind:at:) 

Instance Method

# supplementaryView(forElementKind:at:)

Gets the supplementary view at the specified index path.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func supplementaryView(
    forElementKind elementKind: String,
    at indexPath: IndexPath
) -> UICollectionReusableView?
```

## Parameters 

`elementKind`  

The kind of supplementary view to locate. This value is defined by the layout object. This parameter must not be `nil`.

`indexPath`  

The index path of the supplementary view. This parameter must not be `nil`.

## Return Value

The specified supplementary view, or `nil` if the view could not be found.

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

func visibleSupplementaryViews(ofKind: String) -> [UICollectionReusableView]

Gets an array of the visible supplementary views of the specified kind.

