

- UIKit
- UIPageViewController
-  setViewControllers(\_:direction:animated:completion:) 

Instance Method

# setViewControllers(\_:direction:animated:completion:)

Sets the view controllers to be displayed.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setViewControllers(
    _ viewControllers: [UIViewController]?,
    direction: UIPageViewController.NavigationDirection,
    animated: Bool,
    completion: ((Bool) -> Void)? = nil
)
```

## Parameters 

`viewControllers`  

The view controller or view controllers to be displayed.

`direction`  

The navigation direction.

`animated`  

A Boolean value that indicates whether the transition is to be animated.

`completion`  

A block to be called when the page-turn animation completes.

The block takes the following parameters:

*finished*  
true if the animation finished; false if it was skipped.

## Discussion

The view controllers passed to this method are those that will be visible after the animation has completed. Use a data source to provide additional view controllers to which users navigate.

If the transition style is UIPageViewController.TransitionStyle.pageCurl, the view controllers to pass in the `viewControllers` parameter depends on the spine location and the value of the isDoubleSided property:

| Spine location | Double sided | What to pass |
|----|----|----|
| UIPageViewController.SpineLocation.mid | true | Pass the page to be displayed on the left and the page to be displayed on the right. |
| UIPageViewController.SpineLocation.min or UIPageViewController.SpineLocation.max | true | Pass the front of the page to be displayed and the back of the previously-displayed page. The back is used for the page turning animation. |
| UIPageViewController.SpineLocation.min or UIPageViewController.SpineLocation.max | false | Pass the front of the page to be displayed. |

## See Also

### Providing Content

enum NavigationDirection

Directions for page-turn transitions.

var viewControllers: [UIViewController]?

The view controllers displayed by the page view controller.

var gestureRecognizers: [UIGestureRecognizer]

An array of UIGestureRecognizer objects that are configured to handle user interaction.

