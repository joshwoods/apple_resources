

- UIKit
- UIScrollView
-  isScrollEnabled 

Instance Property

# isScrollEnabled

A Boolean value that determines whether scrolling is enabled.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isScrollEnabled: Bool { get set }
```

## Discussion

The default value is true, which indicates that scrolling is enabled. Setting the value to false disables scrolling.

When scrolling is disabled, the scroll view doesn’t accept touch events; it forwards them up the responder chain.

## See Also

### Configuring the scroll view

var isDirectionalLockEnabled: Bool

A Boolean value that determines whether scrolling is disabled in a particular direction.

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

