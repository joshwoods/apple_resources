

- UIKit
-  UIPageViewControllerDelegate 

Protocol

# UIPageViewControllerDelegate

The delegate of a page view controller must adopt the UIPageViewControllerDelegate protocol. These methods allow the delegate to receive a notification when the device orientation changes and when the user navigates to a new page. For page-curl style transitions, the delegate can provide a different spine location in response to a change in the interface orientation.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIPageViewControllerDelegate : NSObjectProtocol
```

## Topics

### Responding to Page View Controller Events

func pageViewController(UIPageViewController, willTransitionTo: [UIViewController])

Called before a gesture-driven transition begins.

func pageViewController(UIPageViewController, didFinishAnimating: Bool, previousViewControllers: [UIViewController], transitionCompleted: Bool)

Called after a gesture-driven transition completes.

func pageViewController(UIPageViewController, spineLocationFor: UIInterfaceOrientation) -> UIPageViewController.SpineLocation

Returns the spine location for the given orientation.

### Overriding View Rotation Settings

func pageViewControllerSupportedInterfaceOrientations(UIPageViewController) -> UIInterfaceOrientationMask

Returns the complete set of supported interface orientations for the page view controller, as determined by the delegate.

func pageViewControllerPreferredInterfaceOrientationForPresentation(UIPageViewController) -> UIInterfaceOrientation

Returns the preferred orientation for presentation of the page view controller, as determined by the delegate.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Customizing the Page View Behavior

var delegate: (any UIPageViewControllerDelegate)?

The delegate object.

