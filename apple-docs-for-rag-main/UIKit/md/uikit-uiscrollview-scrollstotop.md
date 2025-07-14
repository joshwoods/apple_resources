

- UIKit
- UIScrollView
-  scrollsToTop 

Instance Property

# scrollsToTop

A Boolean value that controls whether the scroll-to-top gesture is enabled.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var scrollsToTop: Bool { get set }
```

## Discussion

The scroll-to-top gesture is a tap on the status bar. When a user makes this gesture, the system asks the scroll view closest to the status bar to scroll to the top. If that scroll view has scrollsToTop set to false, its delegate returns false from scrollViewShouldScrollToTop(_:), or the content is already at the top, nothing happens.

After the scroll view scrolls to the top of the content view, it sends the delegate a scrollViewDidScrollToTop(_:) message.

The default value of this property is true.

### Special considerations

On iPhone, the scroll-to-top gesture has no effect if there’s more than one scroll view onscreen that has scrollsToTop set to true.

## See Also

### Configuring the scroll view

var isScrollEnabled: Bool

A Boolean value that determines whether scrolling is enabled.

var isDirectionalLockEnabled: Bool

A Boolean value that determines whether scrolling is disabled in a particular direction.

var isPagingEnabled: Bool

A Boolean value that determines whether paging is enabled for the scroll view.

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

