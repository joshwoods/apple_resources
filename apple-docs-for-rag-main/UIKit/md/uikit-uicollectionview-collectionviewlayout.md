

- UIKit
- UICollectionView
-  collectionViewLayout 

Instance Property

# collectionViewLayout

The layout used to organize the collected view’s items.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var collectionViewLayout: UICollectionViewLayout { get set }
```

## Discussion

Assigning a new layout object to this property causes the new layout to be applied (without animations) to the collection view’s items.

For more information, see Layouts.

## See Also

### Changing the layout

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

typealias LayoutInteractiveTransitionCompletion

The completion block called at the end of an interactive transition for a collection view.

