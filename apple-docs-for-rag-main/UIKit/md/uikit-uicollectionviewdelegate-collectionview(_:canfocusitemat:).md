

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:canFocusItemAt:) 

Instance Method

# collectionView(\_:canFocusItemAt:)

Asks the delegate whether the item at the specified index path can be focused.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    canFocusItemAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`collectionView`  

The collection view object requesting this information.

`indexPath`  

The index path of an item in the collection view.

## Return Value

true if the item can receive be focused or false if it can not.

## Discussion

You can use this method, or a cell’s canBecomeFocused method, to control which items in the collection view can receive focus. The focus engine calls the cell’s canBecomeFocused method first, the default implementation of which defers to the collection view and this delegate method.

If you do not implement this method, the ability to focus on items depends on whether the collection view’s items are selectable. When the items are selectable, they can also be focused as if this method had returned true; otherwise, they do not receive focus.

## See Also

### Related Documentation

var allowsSelection: Bool

A Boolean value that indicates whether users can select items in the collection view.

### Working with focus

func indexPathForPreferredFocusedView(in: UICollectionView) -> IndexPath?

Asks the delegate for the index path of the cell that should be focused.

func collectionView(UICollectionView, shouldUpdateFocusIn: UICollectionViewFocusUpdateContext) -> Bool

Asks the delegate whether a change in focus should occur.

func collectionView(UICollectionView, didUpdateFocusIn: UICollectionViewFocusUpdateContext, with: UIFocusAnimationCoordinator)

Tells the delegate that a focus update occurred.

func collectionView(UICollectionView, selectionFollowsFocusForItemAt: IndexPath) -> Bool

Asks the delegate whether to relate selection and focus behavior for the cell at the corresponding index path.

