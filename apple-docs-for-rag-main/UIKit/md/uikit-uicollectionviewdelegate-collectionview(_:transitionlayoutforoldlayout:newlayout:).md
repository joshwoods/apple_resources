

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:transitionLayoutForOldLayout:newLayout:) 

Instance Method

# collectionView(\_:transitionLayoutForOldLayout:newLayout:)

Asks for the custom transition layout to use when moving between the specified layouts.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    transitionLayoutForOldLayout fromLayout: UICollectionViewLayout,
    newLayout toLayout: UICollectionViewLayout
) -> UICollectionViewTransitionLayout
```

## Parameters 

`collectionView`  

The collection view whose layout object is changing.

`fromLayout`  

The current layout of the collection view. This is the starting point for the transition.

`toLayout`  

The new layout for the collection view.

## Return Value

The collection view transition layout object to use to perform the transition.

## Discussion

Implement this method if you want to return a custom UICollectionViewTransitionLayout object for use during the transition. A transition layout object lets you customize the behavior of cells and decoration views when transitioning from one layout to the next. Normally, transitioning between layouts causes items to animate directly from their current locations to their new locations. With a transition layout object, you can have objects follow a non linear path, use a different timing algorithm, or move according to incoming touch events.

If your delegate does not implement this method, the collection view creates a standard UICollectionViewTransitionLayout object and uses that object to manage the transition.

## See Also

### Handling layout changes

func collectionView(UICollectionView, targetContentOffsetForProposedContentOffset: CGPoint) -> CGPoint

Gives the delegate an opportunity to customize the content offset for layout changes and animated updates.

func collectionView(UICollectionView, targetIndexPathForMoveOfItemFromOriginalIndexPath: IndexPath, atCurrentIndexPath: IndexPath, toProposedIndexPath: IndexPath) -> IndexPath

Asks the delegate for the index path to use when moving an item.

