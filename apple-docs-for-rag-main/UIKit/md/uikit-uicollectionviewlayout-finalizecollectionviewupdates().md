

- UIKit
- UICollectionViewLayout
-  finalizeCollectionViewUpdates() 

Instance Method

# finalizeCollectionViewUpdates()

Performs any additional animations or clean up needed during a collection view update.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func finalizeCollectionViewUpdates()
```

## Discussion

The collection view calls this method as the last step before proceeding to animate any changes into place. This method is called within the animation block used to perform all of the insertion, deletion, and move animations so you can create additional animations using this method as needed. Otherwise, you can use it to perform any last minute tasks associated with managing your layout object’s state information.

## See Also

### Responding to collection view updates

func prepare(forCollectionViewUpdates: [UICollectionViewUpdateItem])

Notifies the layout object that the contents of the collection view are about to change.

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

func targetIndexPath(forInteractivelyMovingItem: IndexPath, withPosition: CGPoint) -> IndexPath

Retrieves the index path to for an item when it is at the specified location in the collection view’s bounds.

