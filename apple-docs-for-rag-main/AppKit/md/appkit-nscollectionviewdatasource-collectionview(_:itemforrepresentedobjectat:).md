

- AppKit
- NSCollectionViewDataSource
-  collectionView(\_:itemForRepresentedObjectAt:) 

Instance Method

# collectionView(\_:itemForRepresentedObjectAt:)

Asks your data source object to provide the item at the specified location in the collection view.

macOS 10.11+

``` source
@MainActor
func collectionView(
    _ collectionView: NSCollectionView,
    itemForRepresentedObjectAt indexPath: IndexPath
) -> NSCollectionViewItem
```

**Required**

## Parameters 

`collectionView`  

The collection view requesting the information.

`indexPath`  

The index path that specifies the location of the item. This index path contains both the section index and the item index within that section.

## Return Value

A configured item object. You must not return `nil` from this method.

## Discussion

All data source objects must implement this method. Your implementation is responsible for creating, configuring, and returning the appropriate item object based on the specified index path. You do this by calling the makeItem(withIdentifier:for:) method of the collection view to retrieve an empty item object of the appropriate type. After receiving the item object, update its properties with the data from your app’s data structures and return it.

You do not need to set the frame of an item’s view from this method. The collection view gets the item’s location and other layout-related attributes from the layout object during a separate step.

## See Also

### Configuring Items and Supplementary Views

func collectionView(NSCollectionView, viewForSupplementaryElementOfKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> NSView

Asks your data source object to provide the supplementary view at the specified location in a section of the collection view.

