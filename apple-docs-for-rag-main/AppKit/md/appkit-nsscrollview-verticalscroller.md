

- AppKit
- NSScrollView
-  verticalScroller 

Instance Property

# verticalScroller

The scroll view’s vertical scroller.

macOS

``` source
@MainActor
var verticalScroller: NSScroller? { get set }
```

## Discussion

The value of this property is `nil` if the scroll view has no vertical scroller.

You can access the vertical scroller using this property even if the scroll view isn’t currently displaying it. To make sure the scroller is visible, set hasVerticalScroller to true.

## See Also

### Managing Scrollers

var horizontalScroller: NSScroller?

The scroll view’s horizontal scroller.

var hasHorizontalScroller: Bool

A Boolean that indicates whether the scroll view has a horizontal scroller.

var hasVerticalScroller: Bool

A Boolean that indicates whether the scroll view has a vertical scroller.

var autohidesScrollers: Bool

A Boolean that indicates whether the scroll view automatically hides its scroll bars when they are not needed.

