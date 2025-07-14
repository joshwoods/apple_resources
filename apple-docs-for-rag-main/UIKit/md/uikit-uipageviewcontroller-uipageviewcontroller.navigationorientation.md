

- UIKit
- UIPageViewController
-  UIPageViewController.NavigationOrientation 

Enumeration

# UIPageViewController.NavigationOrientation

Orientations for page-turn transitions.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum NavigationOrientation
```

## Topics

### Constants

case horizontal

Horizontal orientation, with pages turning left and right.

case vertical

Vertical orientation, with pages turning up and down.

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

var spineLocation: UIPageViewController.SpineLocation

The location of the spine.

enum SpineLocation

Locations for the spine.

var transitionStyle: UIPageViewController.TransitionStyle

The style used to transition between view controllers.

enum TransitionStyle

Styles for the page-turn transition.

var isDoubleSided: Bool

A Boolean value that indicates whether content appears on the back of pages.

