

- UIKit
- UICollectionViewLayout
-  initialLayoutAttributesForAppearingDecorationElement(ofKind:at:) 

Instance Method

# initialLayoutAttributesForAppearingDecorationElement(ofKind:at:)

Retrieves the starting layout information for a decoration view being inserted into the collection view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func initialLayoutAttributesForAppearingDecorationElement(
    ofKind elementKind: String,
    at decorationIndexPath: IndexPath
) -> UICollectionViewLayoutAttributes?
```

## Parameters 

`elementKind`  

A string that identifies the type of decoration view.

`decorationIndexPath`  

The index path of the item being inserted.

## Return Value

A layout attributes object that describes the position at which to place the corresponding decoration view.

## Discussion

This method is called after the prepare(forCollectionViewUpdates:) method and before the finalizeCollectionViewUpdates() method for any decoration views that are about to be inserted. Your implementation should return the layout information that describes the initial position and state of the view. The collection view uses this information as the starting point for any animations. (The end point of the animation is the view’s new location in the collection view.) If you return `nil`, the layout object uses the item’s final attributes for both the start and end points of the animation.

The default implementation of this method returns `nil`.

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

