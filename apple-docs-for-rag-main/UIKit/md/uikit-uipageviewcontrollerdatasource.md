

- UIKit
-  UIPageViewControllerDataSource 

Protocol

# UIPageViewControllerDataSource

The UIPageViewControllerDataSource protocol is adopted by an object that provides view controllers to the page view controller on an as-needed basis, in response to navigation gestures.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIPageViewControllerDataSource : NSObjectProtocol
```

## Overview

The data source implementation is free to handle this responsibility in any way that is appropriate for your application. In many cases, it should look at the view controller passed to it, determine what content to display, and create the view controllers as they are needed. You may find it helpful to include information such as the page number in the view controller, to simplify the task of determining what content to display.

If both of the methods in Supporting a Page Indicator are implemented and the page view controller’s transition style is UIPageViewController.TransitionStyle.scroll, a page indicator is visible. Both of these methods are called after the setViewControllers(_:direction:animated:completion:) method is called. After gesture-driven navigation, these methods are not called. The index is updated automatically and the number of view controllers is expected to remain constant.

## Topics

### Providing View Controllers

func pageViewController(UIPageViewController, viewControllerBefore: UIViewController) -> UIViewController?

Returns the view controller before the given view controller.

**Required**

func pageViewController(UIPageViewController, viewControllerAfter: UIViewController) -> UIViewController?

Returns the view controller after the given view controller.

**Required**

### Supporting a Page Indicator

func presentationCount(for: UIPageViewController) -> Int

Returns the number of items to be reflected in the page indicator.

func presentationIndex(for: UIPageViewController) -> Int

Returns the index of the selected item to be reflected in the page indicator.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Providing the Page Content

var dataSource: (any UIPageViewControllerDataSource)?

The object that provides view controllers.

