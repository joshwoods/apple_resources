

- AppKit
- NSScrollView
-  autohidesScrollers 

Instance Property

# autohidesScrollers

A Boolean that indicates whether the scroll view automatically hides its scroll bars when they are not needed.

macOS

``` source
@MainActor
var autohidesScrollers: Bool { get set }
```

## Discussion

The horizontal and vertical scroll bars are hidden independently of each other. When the value of this property is true and the content of the scroll view doesn’t extend beyond the size of the clip view on a given axis, the scroller on that axis is removed to leave more room for the content.

Note

The `autohidesScrollers` property introduced in OS X v10.3, while still relevant for legacy-style scrollers, does not apply to the automatic hiding behavior of overlay-style scrollers. The property may still be set, but is ignored by a scroll view that’s using overlay scrollers.

## See Also

### Related Documentation

var scrollerStyle: NSScroller.Style

The scroller style used by the scroll view.

### Managing Scrollers

var horizontalScroller: NSScroller?

The scroll view’s horizontal scroller.

var hasHorizontalScroller: Bool

A Boolean that indicates whether the scroll view has a horizontal scroller.

var verticalScroller: NSScroller?

The scroll view’s vertical scroller.

var hasVerticalScroller: Bool

A Boolean that indicates whether the scroll view has a vertical scroller.

