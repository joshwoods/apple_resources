

- AppKit
- NSScrollView
-  hasVerticalScroller 

Instance Property

# hasVerticalScroller

A Boolean that indicates whether the scroll view has a vertical scroller.

macOS

``` source
@MainActor
var hasVerticalScroller: Bool { get set }
```

## Discussion

When the value of this property is true, the scroll view allocates and displays a vertical scroller as needed. The default value of this property is false.

## See Also

### Managing Scrollers

var horizontalScroller: NSScroller?

The scroll view’s horizontal scroller.

var hasHorizontalScroller: Bool

A Boolean that indicates whether the scroll view has a horizontal scroller.

var verticalScroller: NSScroller?

The scroll view’s vertical scroller.

var autohidesScrollers: Bool

A Boolean that indicates whether the scroll view automatically hides its scroll bars when they are not needed.

