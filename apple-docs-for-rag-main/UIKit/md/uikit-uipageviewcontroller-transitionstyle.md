

- UIKit
- UIPageViewController
-  transitionStyle 

Instance Property

# transitionStyle

The style used to transition between view controllers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var transitionStyle: UIPageViewController.TransitionStyle { get }
```

## Discussion

The value of this property is set when the page view controller is initialized, and cannot be changed.

## See Also

### Display Options

var navigationOrientation: UIPageViewController.NavigationOrientation

The direction along which navigation occurs.

enum NavigationOrientation

Orientations for page-turn transitions.

var spineLocation: UIPageViewController.SpineLocation

The location of the spine.

enum SpineLocation

Locations for the spine.

enum TransitionStyle

Styles for the page-turn transition.

var isDoubleSided: Bool

A Boolean value that indicates whether content appears on the back of pages.

