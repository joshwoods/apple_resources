

- UIKit
- UICollectionViewLayout
-  targetIndexPath(forInteractivelyMovingItem:withPosition:) 

Instance Method

# targetIndexPath(forInteractivelyMovingItem:withPosition:)

Retrieves the index path to for an item when it is at the specified location in the collection view’s bounds.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func targetIndexPath(
    forInteractivelyMovingItem previousIndexPath: IndexPath,
    withPosition position: CGPoint
) -> IndexPath
```

## Parameters 

`previousIndexPath`  

The previous index path of the item. Use this value to identify the item.

`position`  

The target point in the collection view’s bounds. Use this value to compute the new index path for the item.

## Return Value

The index path corresponding to the specified location in the collection view.

## Discussion

During interactive movement of an item, this method maps points in the collection view’s bounds rectangle to index paths that correspond to the locations of those points. The default implementation of this method searches for an existing cell at the specified location and returns the index path of that cell. If there are multiple cells at the same location, the method returns the topmost cell—that is, the cell whose zIndex layout attribute value is greatest.

You can override this method as needed to change how the index path is determined. For example, you might return the index path of the cell that has the lowest zIndex value instead of the highest. If you override this method, you do not need to call `super`.

## See Also

### Responding to collection view updates

func prepare(forCollectionViewUpdates: [UICollectionViewUpdateItem])

Notifies the layout object that the contents of the collection view are about to change.

func finalizeCollectionViewUpdates()

Performs any additional animations or clean up needed during a collection view update.

func indexPathsToInsertForSupplementaryView(ofKind: String) -> [IndexPath]

Retrieves an array of index paths for the supplementary views you want to add to the layout.

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

