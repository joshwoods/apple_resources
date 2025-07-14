

- UIKit
- UICollectionViewDataSource
-  collectionView(\_:canMoveItemAt:) 

Instance Method

# collectionView(\_:canMoveItemAt:)

Asks your data source object whether the specified item can move to another location in the collection view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    canMoveItemAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`collectionView`  

The collection view requesting this information.

`indexPath`  

The index path of the item that the collection view is trying to move.

## Return Value

true if the item is allowed to move, or false if it isn’t.

## Discussion

Use this method to selectively allow or disallow the movement of items within a collection view. If you don’t implement this method, but you do implement the collectionView(_:moveItemAt:to:) method, the collection view allows all items to be reordered.

## See Also

### Reordering items

func collectionView(UICollectionView, moveItemAt: IndexPath, to: IndexPath)

Tells your data source object to move the specified item to its new location.

