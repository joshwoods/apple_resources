

- UIKit
- UIPageViewControllerDelegate
-  pageViewControllerSupportedInterfaceOrientations(\_:) 

Instance Method

# pageViewControllerSupportedInterfaceOrientations(\_:)

Returns the complete set of supported interface orientations for the page view controller, as determined by the delegate.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pageViewControllerSupportedInterfaceOrientations(_ pageViewController: UIPageViewController) -> UIInterfaceOrientationMask
```

## Parameters 

`pageViewController`  

The page view controller.

## Return Value

One of the UIInterfaceOrientationMask constants that represents the set of interface orientations supported by the page view controller.

## See Also

### Related Documentation

var supportedInterfaceOrientations: UIInterfaceOrientationMask

The interface orientations that the view controller supports.

### Overriding View Rotation Settings

func pageViewControllerPreferredInterfaceOrientationForPresentation(UIPageViewController) -> UIInterfaceOrientation

Returns the preferred orientation for presentation of the page view controller, as determined by the delegate.

