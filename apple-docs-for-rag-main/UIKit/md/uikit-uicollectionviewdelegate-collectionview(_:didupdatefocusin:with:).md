

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:didUpdateFocusIn:with:) 

Instance Method

# collectionView(\_:didUpdateFocusIn:with:)

Tells the delegate that a focus update occurred.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    didUpdateFocusIn context: UICollectionViewFocusUpdateContext,
    with coordinator: UIFocusAnimationCoordinator
)
```

## Parameters 

`collectionView`  

The collection view object notifying you of the focus change.

`context`  

The context object containing metadata associated with the focus change. This object contains the index path of the previously focused item and the currently focused item.

`coordinator`  

The animation coordinator to use when creating any additional animations.

## Discussion

The collection view calls this method when a focus-related change occurs. You can use this method to update your app’s state information or to animate changes to your app’s visual appearance.

If you subclass UICollectionView, you can also implement the same behavior by overriding the didUpdateFocus(in:with:) method, which is defined by the UIFocusEnvironment protocol and adopted by all views.

## See Also

### Related Documentation

func didUpdateFocus(in: UIFocusUpdateContext, with: UIFocusAnimationCoordinator)

Called immediately after the system updates the focus to a new view.

**Required**

### Working with focus

func collectionView(UICollectionView, canFocusItemAt: IndexPath) -> Bool

Asks the delegate whether the item at the specified index path can be focused.

func indexPathForPreferredFocusedView(in: UICollectionView) -> IndexPath?

Asks the delegate for the index path of the cell that should be focused.

func collectionView(UICollectionView, shouldUpdateFocusIn: UICollectionViewFocusUpdateContext) -> Bool

Asks the delegate whether a change in focus should occur.

func collectionView(UICollectionView, selectionFollowsFocusForItemAt: IndexPath) -> Bool

Asks the delegate whether to relate selection and focus behavior for the cell at the corresponding index path.

