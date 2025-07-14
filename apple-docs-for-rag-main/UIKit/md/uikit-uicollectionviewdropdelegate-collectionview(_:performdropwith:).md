

- UIKit
- UICollectionViewDropDelegate
-  collectionView(\_:performDropWith:) 

Instance Method

# collectionView(\_:performDropWith:)

Tells your delegate to incorporate the drop data into the collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func collectionView(
    _ collectionView: UICollectionView,
    performDropWith coordinator: any UICollectionViewDropCoordinator
)
```

**Required**

## Parameters 

`collectionView`  

The collection view that received the drop.

`coordinator`  

The coordinator object to use when handling the drop. Use this object to coordinate your custom behavior with the default behavior of the collection view.

## Mentioned in 

Supporting Drag and Drop in Collection Views

## Discussion

Use this method to accept the dropped content and integrate it into your collection view. In your implementation, iterate over the items property of the `coordinator` object and fetch the data from each UIDragItem. Incorporate the data into your collection view’s data source and update the collection view itself by inserting any needed items. When incorporating items, use the methods of the `coordinator` object to animate the transition from the drag item’s preview to the corresponding item in your collection view. For items that you incorporate immediately, you can use the drop(_:to:) or drop(_:toItemAt:) method to perform the animation.

