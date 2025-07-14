

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:shouldUpdateFocusIn:) 

Instance Method

# collectionView(\_:shouldUpdateFocusIn:)

Asks the delegate whether a change in focus should occur.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    shouldUpdateFocusIn context: UICollectionViewFocusUpdateContext
) -> Bool
```

## Parameters 

`collectionView`  

The collection view object requesting this information.

`context`  

The context object containing metadata associated with the focus change. This object contains the index path of the previously focused item and the item targeted to receive focus next. Use this information to determine if the focus change should occur.

## Return Value

true if the focus change should occur or false if it should not.

## Discussion

Before a focus change can occur, the focus engine asks all affected views if such a change should occur. In response, the collection view calls this method to give you the opportunity to allow or prevent the change. Return this method to prevent changes that should not occur. For example, you might use it to ensure that the navigation between cells occurs in a specific order.

If you do not implement this method, the collection view assumes a return value of true.

If you subclass UICollectionView, you can also implement the same behavior by overriding the shouldUpdateFocus(in:) method, which is defined by the UIFocusEnvironment protocol and adopted by all views.

## See Also

### Related Documentation

func shouldUpdateFocus(in: UIFocusUpdateContext) -> Bool

Returns a Boolean value indicating whether the focus engine should allow the focus update described by the specified context to occur.

**Required**

### Working with focus

func collectionView(UICollectionView, canFocusItemAt: IndexPath) -> Bool

Asks the delegate whether the item at the specified index path can be focused.

func indexPathForPreferredFocusedView(in: UICollectionView) -> IndexPath?

Asks the delegate for the index path of the cell that should be focused.

func collectionView(UICollectionView, didUpdateFocusIn: UICollectionViewFocusUpdateContext, with: UIFocusAnimationCoordinator)

Tells the delegate that a focus update occurred.

func collectionView(UICollectionView, selectionFollowsFocusForItemAt: IndexPath) -> Bool

Asks the delegate whether to relate selection and focus behavior for the cell at the corresponding index path.

