

- AppKit
- NSScrollView
-  horizontalScroller 

Instance Property

# horizontalScroller

The scroll view’s horizontal scroller.

macOS

``` source
@MainActor
var horizontalScroller: NSScroller? { get set }
```

## Discussion

The value of this property is `nil` if the scroll view has no horizontal scroller.

You can access the horizontal scroller using this property even if the scroll view isn’t currently displaying it. To make sure the scroller is visible, set hasHorizontalScroller to true.

## See Also

### Managing Scrollers

var hasHorizontalScroller: Bool

A Boolean that indicates whether the scroll view has a horizontal scroller.

var verticalScroller: NSScroller?

The scroll view’s vertical scroller.

var hasVerticalScroller: Bool

A Boolean that indicates whether the scroll view has a vertical scroller.

var autohidesScrollers: Bool

A Boolean that indicates whether the scroll view automatically hides its scroll bars when they are not needed.

