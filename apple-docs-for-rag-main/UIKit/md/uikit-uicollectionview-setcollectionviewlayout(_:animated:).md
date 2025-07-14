

- UIKit
- UICollectionView
-  setCollectionViewLayout(\_:animated:) 

Instance Method

# setCollectionViewLayout(\_:animated:)

Changes the collection view’s layout and optionally animates the change.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setCollectionViewLayout(
    _ layout: UICollectionViewLayout,
    animated: Bool
)
```

## Parameters 

`layout`  

The new layout object for the collection view.

`animated`  

Specify true if you want to animate changes from the current layout to the new layout specified by the `layout` parameter. Specify false to make the change without animations.

## Discussion

This method makes the layout change without further interaction from the user. If you choose to animate the layout change, the animation timing and parameters are controlled by the collection view.

## See Also

### Changing the layout

var collectionViewLayout: UICollectionViewLayout

The layout used to organize the collected view’s items.

func setCollectionViewLayout(UICollectionViewLayout, animated: Bool, completion: ((Bool) -> Void)?)

Changes the collection view’s layout and notifies you when the animations complete.

func startInteractiveTransition(to: UICollectionViewLayout, completion: UICollectionView.LayoutInteractiveTransitionCompletion?) -> UICollectionViewTransitionLayout

Changes the collection view’s current layout using an interactive transition effect.

func finishInteractiveTransition()

Tells the collection view to finish an interactive transition by installing the intended target layout.

func cancelInteractiveTransition()

Tells the collection view to cancel an interactive transition and return to its original layout object.

typealias LayoutInteractiveTransitionCompletion

The completion block called at the end of an interactive transition for a collection view.

