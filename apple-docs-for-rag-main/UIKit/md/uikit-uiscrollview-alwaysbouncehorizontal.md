

- UIKit
- UIScrollView
-  alwaysBounceHorizontal 

Instance Property

# alwaysBounceHorizontal

A Boolean value that determines whether bouncing always occurs when horizontal scrolling reaches the end of the content view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var alwaysBounceHorizontal: Bool { get set }
```

## Discussion

If the value of this property is true and bouncesHorizontally is true, the scroll view allows horizontal dragging even if the content is smaller than the bounds of the scroll view. The default value is false.

## See Also

### Configuring the scroll view

var isScrollEnabled: Bool

A Boolean value that determines whether scrolling is enabled.

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

