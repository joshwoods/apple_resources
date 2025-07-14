

- UIKit
- UISheetPresentationController
-  prefersEdgeAttachedInCompactHeight 

Instance Property

# prefersEdgeAttachedInCompactHeight

A Boolean value that determines whether the sheet attaches to the bottom edge of the screen in a compact-height size class.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var prefersEdgeAttachedInCompactHeight: Bool { get set }
```

## Discussion

The default value is false, which means the sheet defaults to a full screen appearance at compact height. Set this value to true to use an alternate appearance in a compact-height size class, causing the sheet to only attach to the screen on its bottom edge.

## See Also

### Managing the appearance

var prefersGrabberVisible: Bool

A Boolean value that determines whether the sheet shows a grabber at the top.

var prefersPageSizing: Bool

A Boolean value that indicates whether the sheet sizes itself for readable content.

var widthFollowsPreferredContentSizeWhenEdgeAttached: Bool

A Boolean value that determines whether the sheet’s width matches its view controller’s preferred content size.

var preferredCornerRadius: CGFloat?

The corner radius that the sheet attempts to present with.

