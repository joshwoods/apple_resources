

- AppKit
- NSScrollView
-  scrollerStyle 

Instance Property

# scrollerStyle

The scroller style used by the scroll view.

macOS 10.7+

``` source
@MainActor
var scrollerStyle: NSScroller.Style { get set }
```

## Discussion

See NSScroller.Style for possible values.

This setting is automatically set at runtime, based on the user’s preference setting and, if relevant, the set of connected pointing devices and their configured scroll capabilities, as determined by the NSScroller method preferredScrollerStyle.

Setting an scroll view’s scroller style sets the style of both the horizontal and vertical scrollers. If the scroll view subsequently creates or is assigned a new horizontal or vertical scroller, they are assigned the same scroller style assigned to the scroll view.

## See Also

### Scroller Style

var scrollerKnobStyle: NSScroller.KnobStyle

The knob style of scroll views that use the overlay scroller style.

