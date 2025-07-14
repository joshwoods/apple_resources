

- UIKit
- UICollectionView
-  UICollectionView.LayoutInteractiveTransitionCompletion 

Type Alias

# UICollectionView.LayoutInteractiveTransitionCompletion

The completion block called at the end of an interactive transition for a collection view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
typealias LayoutInteractiveTransitionCompletion = (Bool, Bool) -> Void
```

## Discussion

This completion block takes the following parameters:

completed  
A Boolean indicating whether the animations ran to completion.

finish  
A Boolean indicating whether the transition finished or was canceled. This parameter is true if the transition ran to completion and the new layout is installed. It is false if the user canceled the transition and the old layout is installed.

## See Also

### Changing the layout

var collectionViewLayout: UICollectionViewLayout

The layout used to organize the collected view’s items.

func setCollectionViewLayout(UICollectionViewLayout, animated: Bool)

Changes the collection view’s layout and optionally animates the change.

func setCollectionViewLayout(UICollectionViewLayout, animated: Bool, completion: ((Bool) -> Void)?)

Changes the collection view’s layout and notifies you when the animations complete.

func startInteractiveTransition(to: UICollectionViewLayout, completion: UICollectionView.LayoutInteractiveTransitionCompletion?) -> UICollectionViewTransitionLayout

Changes the collection view’s current layout using an interactive transition effect.

func finishInteractiveTransition()

Tells the collection view to finish an interactive transition by installing the intended target layout.

func cancelInteractiveTransition()

Tells the collection view to cancel an interactive transition and return to its original layout object.

