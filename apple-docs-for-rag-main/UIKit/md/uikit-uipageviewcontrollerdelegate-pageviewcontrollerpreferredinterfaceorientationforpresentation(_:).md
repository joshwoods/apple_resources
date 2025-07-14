

- UIKit
- UIPageViewControllerDelegate
-  pageViewControllerPreferredInterfaceOrientationForPresentation(\_:) 

Instance Method

# pageViewControllerPreferredInterfaceOrientationForPresentation(\_:)

Returns the preferred orientation for presentation of the page view controller, as determined by the delegate.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pageViewControllerPreferredInterfaceOrientationForPresentation(_ pageViewController: UIPageViewController) -> UIInterfaceOrientation
```

## Parameters 

`pageViewController`  

The page view controller.

## Return Value

The preferred orientation for presenting the page view controller.

## See Also

### Related Documentation

var preferredInterfaceOrientationForPresentation: UIInterfaceOrientation

The interface orientation to use when presenting the view controller.

### Overriding View Rotation Settings

func pageViewControllerSupportedInterfaceOrientations(UIPageViewController) -> UIInterfaceOrientationMask

Returns the complete set of supported interface orientations for the page view controller, as determined by the delegate.

