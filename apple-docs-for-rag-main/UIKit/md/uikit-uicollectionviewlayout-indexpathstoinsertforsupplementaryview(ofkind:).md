

- UIKit
- UICollectionViewLayout
-  indexPathsToInsertForSupplementaryView(ofKind:) 

Instance Method

# indexPathsToInsertForSupplementaryView(ofKind:)

Retrieves an array of index paths for the supplementary views you want to add to the layout.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func indexPathsToInsertForSupplementaryView(ofKind elementKind: String) -> [IndexPath]
```

## Parameters 

`elementKind`  

The specific type of supplementary view.

## Return Value

An array of NSIndexPath objects indicating the location of the new supplementary views, or an empty array if you don’t want to add any supplementary views.

## Discussion

The collection view calls this method whenever you add cells or sections to the collection view. Implementing this method gives your layout object an opportunity to add new supplementary views to complement the additions.

The collection view calls this method between its calls to prepare(forCollectionViewUpdates:) and finalizeCollectionViewUpdates().

## See Also

### Responding to collection view updates

func prepare(forCollectionViewUpdates: [UICollectionViewUpdateItem])

Notifies the layout object that the contents of the collection view are about to change.

func finalizeCollectionViewUpdates()

Performs any additional animations or clean up needed during a collection view update.

func indexPathsToInsertForDecorationView(ofKind: String) -> [IndexPath]

Retrieves an array of index paths representing the decoration views to add.

func initialLayoutAttributesForAppearingItem(at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the starting layout information for an item being inserted into the collection view.

func initialLayoutAttributesForAppearingSupplementaryElement(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the starting layout information for a supplementary view being inserted into the collection view.

func initialLayoutAttributesForAppearingDecorationElement(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the starting layout information for a decoration view being inserted into the collection view.

func indexPathsToDeleteForSupplementaryView(ofKind: String) -> [IndexPath]

Retrieves an array of index paths representing the supplementary views to remove.

func indexPathsToDeleteForDecorationView(ofKind: String) -> [IndexPath]

Retrieves an array of index paths representing the decoration views to remove.

func finalLayoutAttributesForDisappearingItem(at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the final layout information for an item that is about to be removed from the collection view.

func finalLayoutAttributesForDisappearingSupplementaryElement(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the final layout information for a supplementary view that is about to be removed from the collection view.

func finalLayoutAttributesForDisappearingDecorationElement(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the final layout information for a decoration view that is about to be removed from the collection view.

func targetIndexPath(forInteractivelyMovingItem: IndexPath, withPosition: CGPoint) -> IndexPath

Retrieves the index path to for an item when it is at the specified location in the collection view’s bounds.

