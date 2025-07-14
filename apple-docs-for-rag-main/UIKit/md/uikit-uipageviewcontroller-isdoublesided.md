

- UIKit
- UIPageViewController
-  isDoubleSided 

Instance Property

# isDoubleSided

A Boolean value that indicates whether content appears on the back of pages.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isDoubleSided: Bool { get set }
```

## Discussion

The default value for this property is false.

If the back of pages has no content (the value is false), then the content on the front of the page will partially show through to the back when turning pages.

If the spine is located in the middle, the value must be true. Setting it to false with the spine located in the middle raises an exception.

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

var transitionStyle: UIPageViewController.TransitionStyle

The style used to transition between view controllers.

enum TransitionStyle

Styles for the page-turn transition.

