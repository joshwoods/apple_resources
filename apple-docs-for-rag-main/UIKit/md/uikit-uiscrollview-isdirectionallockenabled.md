

- UIKit
- UIScrollView
-  isDirectionalLockEnabled 

Instance Property

# isDirectionalLockEnabled

A Boolean value that determines whether scrolling is disabled in a particular direction.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isDirectionalLockEnabled: Bool { get set }
```

## Discussion

If this property is false, scrolling is permitted in both horizontal and vertical directions. If this property is true and the user begins dragging in one general direction (horizontally or vertically), the scroll view disables scrolling in the other direction. If the drag direction is diagonal, then scrolling doesn’t lock and the user can drag in any direction until the drag completes. The default value is false.

## See Also

### Configuring the scroll view

var isScrollEnabled: Bool

A Boolean value that determines whether scrolling is enabled.

var isPagingEnabled: Bool

A Boolean value that determines whether paging is enabled for the scroll view.

var scrollsToTop: Bool

A Boolean value that controls whether the scroll-to-top gesture is enabled.

var bounces: Bool

A Boolean value that controls whether the scroll view bounces past the edge of content and back again.

var bouncesHorizontally: Bool

A Boolean value that determines whether the scroll view bounces when it reaches the ends of its horizontal axis.

var bouncesVertically: Bool

A Boolean value that determines whether the scroll view bounces when it reaches the ends of its vertical axis.

var alwaysBounceVertical: Bool

A Boolean value that determines whether bouncing always occurs when vertical scrolling reaches the end of the content.

var alwaysBounceHorizontal: Bool

A Boolean value that determines whether bouncing always occurs when horizontal scrolling reaches the end of the content view.

