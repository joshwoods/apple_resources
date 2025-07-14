

- UIKit
- UISheetPresentationController
-  widthFollowsPreferredContentSizeWhenEdgeAttached 

Instance Property

# widthFollowsPreferredContentSizeWhenEdgeAttached

A Boolean value that determines whether the sheet’s width matches its view controller’s preferred content size.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var widthFollowsPreferredContentSizeWhenEdgeAttached: Bool { get set }
```

## Discussion

The default value is false, which means the sheet’s width equals the width of its container’s safe area. Set this value to true to use your view controller’s preferredContentSize to determine the width of the sheet instead.

This property doesn’t have an effect when the sheet is in a compact-width and regular-height size class, or when prefersEdgeAttachedInCompactHeight is false.

## See Also

### Managing the appearance

var prefersGrabberVisible: Bool

A Boolean value that determines whether the sheet shows a grabber at the top.

var prefersPageSizing: Bool

A Boolean value that indicates whether the sheet sizes itself for readable content.

var prefersEdgeAttachedInCompactHeight: Bool

A Boolean value that determines whether the sheet attaches to the bottom edge of the screen in a compact-height size class.

var preferredCornerRadius: CGFloat?

The corner radius that the sheet attempts to present with.

