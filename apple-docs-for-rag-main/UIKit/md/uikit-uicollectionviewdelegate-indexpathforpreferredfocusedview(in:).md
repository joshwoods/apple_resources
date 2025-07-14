

- UIKit
- UICollectionViewDelegate
-  indexPathForPreferredFocusedView(in:) 

Instance Method

# indexPathForPreferredFocusedView(in:)

Asks the delegate for the index path of the cell that should be focused.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func indexPathForPreferredFocusedView(in collectionView: UICollectionView) -> IndexPath?
```

## Parameters 

`collectionView`  

The collection view object requesting this information.

## Return Value

The index path of the preferred cell. The index path you specify must correspond to a valid cell in the collection view.

## Discussion

When focus is about to change to a collection view, the collection view must pick which of its subviews should receive that focus. If the collection view’s remembersLastFocusedIndexPath property is set to true, the collection view returns the index path of the cell that was last focused. If the remembersLastFocusedIndexPath property is false, or if there is no saved index path because no cell was previously focused, the collection view calls this method so that you can specify which cell should receive focus. If you do not implement this method, the collection view returns an appropriate cell.

The effects of this method may be ignored during or immediately after a view controller transition, such as a presentation dismissal or navigation stack pop. In such cases, the view controller attempts to restore focus to the item that was focused prior to the transition (for example, prior to the view controller being presented or pushed), which can take precedence over the effects of this method. To learn how to control or disable this behavior in the view controller, see restoresFocusAfterTransition.

If you subclass UICollectionView, you can also implement the same behavior by overriding the preferredFocusEnvironments property, which is defined by the UIFocusEnvironment protocol and adopted by all views.

## See Also

### Related Documentation

var preferredFocusedView: UIView?

Specifies the view that should be focused if this environment is focused.

Deprecated

### Working with focus

func collectionView(UICollectionView, canFocusItemAt: IndexPath) -> Bool

Asks the delegate whether the item at the specified index path can be focused.

func collectionView(UICollectionView, shouldUpdateFocusIn: UICollectionViewFocusUpdateContext) -> Bool

Asks the delegate whether a change in focus should occur.

func collectionView(UICollectionView, didUpdateFocusIn: UICollectionViewFocusUpdateContext, with: UIFocusAnimationCoordinator)

Tells the delegate that a focus update occurred.

func collectionView(UICollectionView, selectionFollowsFocusForItemAt: IndexPath) -> Bool

Asks the delegate whether to relate selection and focus behavior for the cell at the corresponding index path.

