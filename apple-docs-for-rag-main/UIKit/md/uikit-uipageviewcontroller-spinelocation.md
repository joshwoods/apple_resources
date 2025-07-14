

- UIKit
- UIPageViewController
-  spineLocation 

Instance Property

# spineLocation

The location of the spine.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var spineLocation: UIPageViewController.SpineLocation { get }
```

## Discussion

The value of this property is set with the spineLocation key when the page view controller is initialized, and can be changed by returning the new value from the pageViewController(_:spineLocationFor:) method of the delegate.

## See Also

### Display Options

var navigationOrientation: UIPageViewController.NavigationOrientation

The direction along which navigation occurs.

enum NavigationOrientation

Orientations for page-turn transitions.

enum SpineLocation

Locations for the spine.

var transitionStyle: UIPageViewController.TransitionStyle

The style used to transition between view controllers.

enum TransitionStyle

Styles for the page-turn transition.

var isDoubleSided: Bool

A Boolean value that indicates whether content appears on the back of pages.

