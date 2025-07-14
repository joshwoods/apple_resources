

- AppKit
- NSCollectionViewDataSource
-  collectionView(\_:viewForSupplementaryElementOfKind:at:) 

Instance Method

# collectionView(\_:viewForSupplementaryElementOfKind:at:)

Asks your data source object to provide the supplementary view at the specified location in a section of the collection view.

macOS 10.10+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    viewForSupplementaryElementOfKind kind: NSCollectionView.SupplementaryElementKind,
    at indexPath: IndexPath
) -> NSView
```

## Parameters 

`collectionView`  

The collection view requesting the information.

`kind`  

The kind of supplementary view to provide. The value of this string is defined by the current layout object associated with the collection view. Layouts may define additional views to add visual content that is unrelated to specific items.

`indexPath`  

The index path that identifies the section in which to place the supplementary view.

## Return Value

A configured view object. You must not return `nil` from this method.

## Discussion

Implement this method if the collection view’s layout object supports supplementary views. Your implementation is responsible for creating, configuring, and returning an appropriate view. You do this by calling the makeSupplementaryView(ofKind:withIdentifier:for:) method of the collection view to retrieve an unconfigured view of the appropriate type. After receiving the view, update its properties and content using your app’s data structures and return it.

You do not need to set the location of supplementary views inside the collection view’s bounds. The collection view gets the view’s location and other layout-related attributes from the layout object during a separate step.

## See Also

### Configuring Items and Supplementary Views

func collectionView(NSCollectionView, itemForRepresentedObjectAt: IndexPath) -> NSCollectionViewItem

Asks your data source object to provide the item at the specified location in the collection view.

**Required**

