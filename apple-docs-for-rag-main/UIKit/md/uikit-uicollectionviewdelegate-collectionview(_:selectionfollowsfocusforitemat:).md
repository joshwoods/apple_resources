

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:selectionFollowsFocusForItemAt:) 

Instance Method

# collectionView(\_:selectionFollowsFocusForItemAt:)

Asks the delegate whether to relate selection and focus behavior for the cell at the corresponding index path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    selectionFollowsFocusForItemAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`collectionView`  

The collection view making the request.

`indexPath`  

The index path of the cell to determine selection and focus behavior for.

## Return Value

true if you want to automatically select the cell at the specified index path when focus moves to it; otherwise, false.

## Discussion

If the collection view’s selectionFollowsFocus property is true and you return false from this delegate method, focus still moves to the cell when the user selects it. However, when focus moves to the cell, the cell doesn’t automatically select.

## See Also

### Working with focus

func collectionView(UICollectionView, canFocusItemAt: IndexPath) -> Bool

Asks the delegate whether the item at the specified index path can be focused.

func indexPathForPreferredFocusedView(in: UICollectionView) -> IndexPath?

Asks the delegate for the index path of the cell that should be focused.

func collectionView(UICollectionView, shouldUpdateFocusIn: UICollectionViewFocusUpdateContext) -> Bool

Asks the delegate whether a change in focus should occur.

func collectionView(UICollectionView, didUpdateFocusIn: UICollectionViewFocusUpdateContext, with: UIFocusAnimationCoordinator)

Tells the delegate that a focus update occurred.

