

- UIKit
- UIPageViewControllerDelegate
-  pageViewController(\_:didFinishAnimating:previousViewControllers:transitionCompleted:) 

Instance Method

# pageViewController(\_:didFinishAnimating:previousViewControllers:transitionCompleted:)

Called after a gesture-driven transition completes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func pageViewController(
    _ pageViewController: UIPageViewController,
    didFinishAnimating finished: Bool,
    previousViewControllers: [UIViewController],
    transitionCompleted completed: Bool
)
```

## Parameters 

`pageViewController`  

The page view controller.

`finished`  

true if the animation finished; otherwise, false.

`previousViewControllers`  

The view controllers prior to the transition.

`completed`  

true if the user completed the page-turn gesture; otherwise, false.

## Discussion

Use the `completed` parameter to distinguish between a transition that completed (the page was turned) and a transition that the user aborted (the page was not turned).

The value of the `previousViewControllers` parameter is the same as what the viewControllers method would have returned prior to the page turn.

## See Also

### Responding to Page View Controller Events

func pageViewController(UIPageViewController, willTransitionTo: [UIViewController])

Called before a gesture-driven transition begins.

func pageViewController(UIPageViewController, spineLocationFor: UIInterfaceOrientation) -> UIPageViewController.SpineLocation

Returns the spine location for the given orientation.

