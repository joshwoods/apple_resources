

- UIKit
- UIPageViewController
-  UIPageViewController.SpineLocation 

Enumeration

# UIPageViewController.SpineLocation

Locations for the spine.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum SpineLocation
```

## Overview

To set the spine location, wrap one of these constants in an NSNumber object and set it as the value for the spineLocation key in the options dictionary passed to the init(transitionStyle:navigationOrientation:options:) method.

## Topics

### Constants

case none

No spine.

case min

Spine at the left or top edge of the screen.

case mid

Spine in the middle or the screen.

case max

Spine at the right or bottom edge of the screen.

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

var transitionStyle: UIPageViewController.TransitionStyle

The style used to transition between view controllers.

enum TransitionStyle

Styles for the page-turn transition.

var isDoubleSided: Bool

A Boolean value that indicates whether content appears on the back of pages.

