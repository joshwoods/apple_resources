

- UIKit
- UIPageViewController
-  init(transitionStyle:navigationOrientation:options:) 

Initializer

# init(transitionStyle:navigationOrientation:options:)

Initializes a newly created page view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    transitionStyle style: UIPageViewController.TransitionStyle,
    navigationOrientation: UIPageViewController.NavigationOrientation,
    options: [UIPageViewController.OptionsKey : Any]? = nil
)
```

## Parameters 

`style`  

The style for transitions between pages.

`navigationOrientation`  

The orientation of the page-by-page navigation.

`options`  

A dictionary of options. For keys, see UIPageViewController.OptionsKey.

## Return Value

The initialized page view controller.

## Discussion

After initialization, use the setViewControllers(_:direction:animated:completion:) method to set the initial view controllers.

## See Also

### Creating a page view controller

init?(coder: NSCoder)

Creates a page view controller from data in an unarchiver.

struct OptionsKey

Keys for creating the page view controller.

