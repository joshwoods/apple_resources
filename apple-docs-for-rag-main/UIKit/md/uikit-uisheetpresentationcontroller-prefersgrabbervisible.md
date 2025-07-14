

- UIKit
- UISheetPresentationController
-  prefersGrabberVisible 

Instance Property

# prefersGrabberVisible

A Boolean value that determines whether the sheet shows a grabber at the top.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor
var prefersGrabberVisible: Bool { get set }
```

## Discussion

The default value is false, which means the sheet doesn’t show a grabber. A *grabber* is a visual affordance that indicates that a sheet is resizable. Showing a grabber may be useful when it isn’t apparent that a sheet can resize or when the sheet can’t dismiss interactively.

Set this value to true for the system to draw a grabber in the standard system-defined location. The system automatically hides the grabber at appropriate times, like when the sheet is full screen in a compact-height size class or when another sheet presents on top of it.

## See Also

### Managing the appearance

var prefersPageSizing: Bool

A Boolean value that indicates whether the sheet sizes itself for readable content.

var prefersEdgeAttachedInCompactHeight: Bool

A Boolean value that determines whether the sheet attaches to the bottom edge of the screen in a compact-height size class.

var widthFollowsPreferredContentSizeWhenEdgeAttached: Bool

A Boolean value that determines whether the sheet’s width matches its view controller’s preferred content size.

var preferredCornerRadius: CGFloat?

The corner radius that the sheet attempts to present with.

