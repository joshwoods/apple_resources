

- UIKit
- UIPageViewController
-  dataSource 

Instance Property

# dataSource

The object that provides view controllers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var dataSource: (any UIPageViewControllerDataSource)? { get set }
```

## Discussion

Methods of the data source are called in response to gesture-based navigation. If the value of this property is `nil`, then gesture-based navigation is disabled.

## See Also

### Providing the Page Content

protocol UIPageViewControllerDataSource

The UIPageViewControllerDataSource protocol is adopted by an object that provides view controllers to the page view controller on an as-needed basis, in response to navigation gestures.

