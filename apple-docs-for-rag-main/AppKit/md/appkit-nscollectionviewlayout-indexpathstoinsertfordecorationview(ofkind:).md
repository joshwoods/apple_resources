

- AppKit
- NSCollectionViewLayout
-  indexPathsToInsertForDecorationView(ofKind:) 

Instance Method

# indexPathsToInsertForDecorationView(ofKind:)

Returns the index paths for any decoration views that the layout object wants to add to the collection view.

macOS

``` source
@MainActor
func indexPathsToInsertForDecorationView(ofKind elementKind: NSCollectionView.DecorationElementKind) -> Set
```

## Parameters 

`elementKind`  

The type of the decoration views to add.

## Return Value

The set of NSIndexPath objects representing the decoration views to insert, or an empty array if you do not want to insert any decoration views.

## Discussion

When your app inserts or deletes items or sections in the collection view, the collection view calls this method for each of the layout’s registered decoration view types. The default implementation returns an empty array, but you can override it and return index paths for each decoration view you want to add. For example, when a section is added, you might want to add the decoration views that are used to adorn that section. In that case, you would add index paths to the array that contain the section numbers that were added.

The index paths you return should always contain a valid section number, but the item number is optional. The item number is necessary only if you support multiple decoration views of the same type in a single section. If you do, your layout object can use the item numbers internally to differentiate the decoration views.

Subclasses are expected to override this method, as needed, and provide any appropriate index paths.

## See Also

### Responding to Collection View Updates

func prepare(forCollectionViewUpdates: [NSCollectionViewUpdateItem])

Performs needed tasks before items are inserted, deleted, or moved within the collection view.

func finalizeCollectionViewUpdates()

Performs needed steps after items are inserted, deleted, or moved within a collection view.

func indexPathsToInsertForSupplementaryView(ofKind: NSCollectionView.SupplementaryElementKind) -> Set&lt;IndexPath>

Returns the index paths for any supplementary views that the layout object wants to add to the collection view.

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

func finalLayoutAttributesForDisappearingItem(at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the ending layout information for an item being removed from the collection view.

func finalLayoutAttributesForDisappearingSupplementaryElement(ofKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the ending layout information for a supplementary view being removed from the collection view.

func finalLayoutAttributesForDisappearingDecorationElement(ofKind: NSCollectionView.DecorationElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the ending layout information for a decoration view being removed from the collection view.

