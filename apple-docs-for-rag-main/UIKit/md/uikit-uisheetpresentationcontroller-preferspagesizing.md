

- UIKit
- UISheetPresentationController
-  prefersPageSizing 

Instance Property

# prefersPageSizing

A Boolean value that indicates whether the sheet sizes itself for readable content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
var prefersPageSizing: Bool { get set }
```

## Discussion

The default value is true. The default value indicates the sheet uses UIModalPresentationStyle.pageSheet behavior, in which the sheet width follows the readable width.

When the value is set to false, the sheet uses UIModalPresentationStyle.formSheet behavior, in which the sheet size follows the presented view controller’s preferredContentSize.

## See Also

### Managing the appearance

var prefersGrabberVisible: Bool

A Boolean value that determines whether the sheet shows a grabber at the top.

var prefersEdgeAttachedInCompactHeight: Bool

A Boolean value that determines whether the sheet attaches to the bottom edge of the screen in a compact-height size class.

var widthFollowsPreferredContentSizeWhenEdgeAttached: Bool

A Boolean value that determines whether the sheet’s width matches its view controller’s preferred content size.

var preferredCornerRadius: CGFloat?

The corner radius that the sheet attempts to present with.

