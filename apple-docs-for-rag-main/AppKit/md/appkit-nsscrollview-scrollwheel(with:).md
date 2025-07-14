

- AppKit
- NSScrollView
-  scrollWheel(with:) 

Instance Method

# scrollWheel(with:)

Scrolls the receiver up or down, in response to the user moving the mouse’s scroll wheel specified by `theEvent`.

macOS

``` source
@MainActor
func scrollWheel(with event: NSEvent)
```

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

var scrollsDynamically: Bool

A Boolean that indicates whether the scroll view redraws its document view while scrolling continuously.

