

- UIKit
- UICollectionView
-  startInteractiveTransition(to:completion:) 

Instance Method

# startInteractiveTransition(to:completion:)

Changes the collection view’s current layout using an interactive transition effect.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func startInteractiveTransition(
    to layout: UICollectionViewLayout,
    completion: UICollectionView.LayoutInteractiveTransitionCompletion? = nil
) -> UICollectionViewTransitionLayout
```

## Parameters 

`layout`  

The new layout object for the collected views. This is the layout that you want the collection view to use after the interactive transition is done.

`completion`  

A completion handler to execute after the transition finishes.

## Return Value

The intermediate transition layout object responsible for managing the interactive transition behavior.

## Discussion

Call this method when you want to change the layout of your collection view using an intermediate transition. When you call this method, the collection view quietly makes the returned transition layout object its current layout object. It is your responsibility to set up a gesture recognizer or other touch-event handling code to track the transition progress. As progress changes, update the transitionProgress property of the transition layout object and invalidate the layout. Invalidating its layout causes the transition layout object to update the position of items based on the new progress value.

When your event-handling code determines that the user has finished the transition to the new layout, call the finishInteractiveTransition() method. If your code determines that the user has canceled the transition, call the cancelInteractiveTransition() method to revert the changes instead. Calling either of these methods removes the transition layout object from the collection view and installs the appropriate target layout object.

This method returns an instance of the UICollectionViewTransitionLayout class by default. If you want it to return a custom transition object instead, implement the collectionView(_:transitionLayoutForOldLayout:newLayout:) method of your collection view delegate and use that method to return your custom object.

## See Also

### Changing the layout

var collectionViewLayout: UICollectionViewLayout

The layout used to organize the collected view’s items.

func setCollectionViewLayout(UICollectionViewLayout, animated: Bool)

Changes the collection view’s layout and optionally animates the change.

func setCollectionViewLayout(UICollectionViewLayout, animated: Bool, completion: ((Bool) -> Void)?)

Changes the collection view’s layout and notifies you when the animations complete.

func finishInteractiveTransition()

Tells the collection view to finish an interactive transition by installing the intended target layout.

func cancelInteractiveTransition()

Tells the collection view to cancel an interactive transition and return to its original layout object.

typealias LayoutInteractiveTransitionCompletion

The completion block called at the end of an interactive transition for a collection view.

