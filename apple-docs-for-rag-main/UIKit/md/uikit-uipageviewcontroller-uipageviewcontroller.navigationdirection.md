

- UIKit
- UIPageViewController
-  UIPageViewController.NavigationDirection 

Enumeration

# UIPageViewController.NavigationDirection

Directions for page-turn transitions.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum NavigationDirection
```

## Overview

For horizontal navigation, pages turn from the right side of the screen to the left as you navigate forward.

For vertical navigation, pages turn from the bottom of the screen to the top as you navigate forward.

## Topics

### Constants

case forward

Navigation to the next page.

case reverse

Navigation to the previous page.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Providing Content

func setViewControllers([UIViewController]?, direction: UIPageViewController.NavigationDirection, animated: Bool, completion: ((Bool) -> Void)?)

Sets the view controllers to be displayed.

var viewControllers: [UIViewController]?

The view controllers displayed by the page view controller.

var gestureRecognizers: [UIGestureRecognizer]

An array of UIGestureRecognizer objects that are configured to handle user interaction.

