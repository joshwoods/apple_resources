

- UIKit
- UIPageViewControllerDelegate
-  pageViewController(\_:spineLocationFor:) 

Instance Method

# pageViewController(\_:spineLocationFor:)

Returns the spine location for the given orientation.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pageViewController(
    _ pageViewController: UIPageViewController,
    spineLocationFor orientation: UIInterfaceOrientation
) -> UIPageViewController.SpineLocation
```

## Parameters 

`pageViewController`  

The page view controller

`orientation`  

The new orientation.

## Return Value

The spine location.

## Discussion

Use this method to change the spine location when the device orientation changes, as well as setting new view controllers and changing the double-sided state.

This method is called only if the transition style is UIPageViewController.TransitionStyle.pageCurl.

## See Also

### Responding to Page View Controller Events

func pageViewController(UIPageViewController, willTransitionTo: [UIViewController])

Called before a gesture-driven transition begins.

func pageViewController(UIPageViewController, didFinishAnimating: Bool, previousViewControllers: [UIViewController], transitionCompleted: Bool)

Called after a gesture-driven transition completes.

