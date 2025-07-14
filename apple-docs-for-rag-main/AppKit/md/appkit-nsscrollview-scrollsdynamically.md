

- AppKit
- NSScrollView
-  scrollsDynamically 

Instance Property

# scrollsDynamically

A Boolean that indicates whether the scroll view redraws its document view while scrolling continuously.

macOS

``` source
@MainActor
var scrollsDynamically: Bool { get set }
```

## Discussion

When the value of this property is true, the scroll view redraws its document view while scrolling. When the value of this property isfalse, the scroll view redraws only when the scroller knob is released. The default value of this property is true.

## See Also

### Setting Scrolling Behavior

var lineScroll: CGFloat

The scroll view’s line by line scroll amount.

var horizontalLineScroll: CGFloat

The scroll view’s horizontal line by line scroll amount.

var verticalLineScroll: CGFloat

The scroll view’s vertical line by line scroll amount.

var pageScroll: CGFloat

The amount of the document view kept visible when scrolling page by page.

var horizontalPageScroll: CGFloat

The amount of the document view kept visible when scrolling horizontally page by page.

var verticalPageScroll: CGFloat

The amount of the document view kept visible when scrolling vertically page by page.

func scrollWheel(with: NSEvent)

Scrolls the receiver up or down, in response to the user moving the mouse’s scroll wheel specified by `theEvent`.

