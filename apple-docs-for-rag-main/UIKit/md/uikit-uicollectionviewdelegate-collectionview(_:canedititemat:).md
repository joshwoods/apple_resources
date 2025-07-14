

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:canEditItemAt:) 

Instance Method

# collectionView(\_:canEditItemAt:)

Determines whether the specified item is editable.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    canEditItemAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`collectionView`  

The collection view object requesting this information.

`indexPath`  

An index path locating an item in the collection view.

## Return Value

Returns true if the item is editable, false if it’s not. The default value is true.

