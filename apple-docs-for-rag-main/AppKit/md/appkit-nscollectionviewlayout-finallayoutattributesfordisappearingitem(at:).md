

- AppKit
- NSCollectionViewLayout
-  finalLayoutAttributesForDisappearingItem(at:) 

Instance Method

# finalLayoutAttributesForDisappearingItem(at:)

Returns the ending layout information for an item being removed from the collection view.

macOS

``` source
@MainActor
func finalLayoutAttributesForDisappearingItem(at itemIndexPath: IndexPath) -> NSCollectionViewLayoutAttributes?
```

## Parameters 

`itemIndexPath`  

The index path of the item being removed. You can use this path to retrieve any relevant information from the collection view’s data source.

## Return Value

The layout attributes object that describes the item’s position and properties at the end of animations.

## Discussion

When your app removes items from the collection view, the collection view calls this method for each item you remove. Use this method to specify the layout attributes of the item after it has been removed. For example, you might return attributes that position the item offscreen or set its final alpha to `0`. The collection view uses the attributes you return as the end point for any animations. (The start point of the animation is the item’s current location and attributes.) If you return `nil`, the layout uses the item’s current attributes for both the start point and end point of the animation.

The default implementation of this method returns `nil`. Subclasses are expected to override this method, as needed, and provide any final attributes.

## See Also

### Responding to Collection View Updates

func prepare(forCollectionViewUpdates: [NSCollectionViewUpdateItem])

Performs needed tasks before items are inserted, deleted, or moved within the collection view.

func finalizeCollectionViewUpdates()

Performs needed steps after items are inserted, deleted, or moved within a collection view.

func indexPathsToInsertForSupplementaryView(ofKind: NSCollectionView.SupplementaryElementKind) -> Set&lt;IndexPath>

Returns the index paths for any supplementary views that the layout object wants to add to the collection view.

func indexPathsToInsertForDecorationView(ofKind: NSCollectionView.DecorationElementKind) -> Set&lt;IndexPath>

Returns the index paths for any decoration views that the layout object wants to add to the collection view.

func initialLayoutAttributesForAppearingItem(at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the starting layout information for an item being inserted into the collection view.

func initialLayoutAttributesForAppearingSupplementaryElement(ofKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the starting layout information for a supplementary view being added to the collection view.

func initialLayoutAttributesForAppearingDecorationElement(ofKind: NSCollectionView.DecorationElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the starting layout information for a decoration view being added to the collection view.

func indexPathsToDeleteForSupplementaryView(ofKind: NSCollectionView.SupplementaryElementKind) -> Set&lt;IndexPath>

Returns the index paths for any supplementary views that the layout object wants to remove from the collection view.

func indexPathsToDeleteForDecorationView(ofKind: NSCollectionView.DecorationElementKind) -> Set&lt;IndexPath>

Returns index paths for any decoration views that the layout object wants to remove from the collection view.

func finalLayoutAttributesForDisappearingSupplementaryElement(ofKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the ending layout information for a supplementary view being removed from the collection view.

func finalLayoutAttributesForDisappearingDecorationElement(ofKind: NSCollectionView.DecorationElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the ending layout information for a decoration view being removed from the collection view.

