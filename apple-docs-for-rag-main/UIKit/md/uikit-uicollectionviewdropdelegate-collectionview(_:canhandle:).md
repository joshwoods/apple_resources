

- UIKit
- UICollectionViewDropDelegate
-  collectionView(\_:canHandle:) 

Instance Method

# collectionView(\_:canHandle:)

Asks your delegate whether the collection view can accept a drop with the specified type of data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    canHandle session: any UIDropSession
) -> Bool
```

## Parameters 

`collectionView`  

The collection view that’s attempting to handle the drop.

`session`  

The drop session object containing information about the type of data being dragged.

## Return Value

true if the collection view can accept the dragged data or false if it cannot.

## Mentioned in 

Supporting Drag and Drop in Collection Views

## Discussion

Implement this method when you want to dynamically determine whether to accept dropped data in your collection view. In your implementation, check the type of the dragged data and return a Boolean value indicating whether you can accept the drop. For example, you might call the hasItemsConforming(toTypeIdentifiers:) method of the session object to determine whether it contains data that your app can accept.

If you don’t implement this method, the collection view assumes a return value of true. If you return false from this method, the collection view doesn’t call any more methods of your drop delegate for the given session.

