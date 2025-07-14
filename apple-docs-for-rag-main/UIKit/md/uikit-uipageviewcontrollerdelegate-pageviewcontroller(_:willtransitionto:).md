

- UIKit
- UIPageViewControllerDelegate
-  pageViewController(\_:willTransitionTo:) 

Instance Method

# pageViewController(\_:willTransitionTo:)

Called before a gesture-driven transition begins.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func pageViewController(
    _ pageViewController: UIPageViewController,
    willTransitionTo pendingViewControllers: [UIViewController]
)
```

## Parameters 

`pageViewController`  

The page view controller.

`pendingViewControllers`  

The view controllers that are being transitioned to.

## Discussion

If the user aborts the navigation gesture, the transition doesn’t complete and the view controllers stay the same.

## See Also

### Responding to Page View Controller Events

func pageViewController(UIPageViewController, didFinishAnimating: Bool, previousViewControllers: [UIViewController], transitionCompleted: Bool)

Called after a gesture-driven transition completes.

func pageViewController(UIPageViewController, spineLocationFor: UIInterfaceOrientation) -> UIPageViewController.SpineLocation

Returns the spine location for the given orientation.

