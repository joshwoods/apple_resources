

- UIKit
- UIPageViewControllerDataSource
-  pageViewController(\_:viewControllerBefore:) 

Instance Method

# pageViewController(\_:viewControllerBefore:)

Returns the view controller before the given view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func pageViewController(
    _ pageViewController: UIPageViewController,
    viewControllerBefore viewController: UIViewController
) -> UIViewController?
```

**Required**

## Parameters 

`pageViewController`  

The page view controller

`viewController`  

The view controller that the user navigated away from.

## Return Value

The view controller before the given view controller, or `nil` to indicate that there is no previous view controller.

## See Also

### Providing View Controllers

func pageViewController(UIPageViewController, viewControllerAfter: UIViewController) -> UIViewController?

Returns the view controller after the given view controller.

**Required**

