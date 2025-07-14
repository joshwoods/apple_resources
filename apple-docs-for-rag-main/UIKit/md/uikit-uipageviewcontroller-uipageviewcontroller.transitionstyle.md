

- UIKit
- UIPageViewController
-  UIPageViewController.TransitionStyle 

Enumeration

# UIPageViewController.TransitionStyle

Styles for the page-turn transition.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum TransitionStyle
```

## Topics

### Constants

case pageCurl

Page curl transition style.

case scroll

Scrolling transition style.

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

var isDoubleSided: Bool

A Boolean value that indicates whether content appears on the back of pages.

