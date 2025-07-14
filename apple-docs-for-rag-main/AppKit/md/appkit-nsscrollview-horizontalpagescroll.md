

- AppKit
- NSScrollView
-  horizontalPageScroll 

Instance Property

# horizontalPageScroll

The amount of the document view kept visible when scrolling horizontally page by page.

macOS

``` source
@MainActor
var horizontalPageScroll: CGFloat { get set }
```

## Discussion

The value of this property is the amount of the document view kept visible when scrolling horizontally page by page, expressed in the content view’s coordinate system. This value is used when the user clicks the scroll arrows on the horizontal scroll bar while holding down the Option key.

This amount expresses the context that remains when the receiver scrolls by one page, allowing the user to orient to the new display. It differs from the line scroll amount, which indicates how far the document view moves. The page scroll amount is the amount common to the content view before and after the document view is scrolled by one page. Thus, setting the page scroll amount to `0.0` implies that the entire visible portion of the document view is replaced when a page scroll occurs.

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

var verticalPageScroll: CGFloat

The amount of the document view kept visible when scrolling vertically page by page.

var scrollsDynamically: Bool

A Boolean that indicates whether the scroll view redraws its document view while scrolling continuously.

func scrollWheel(with: NSEvent)

Scrolls the receiver up or down, in response to the user moving the mouse’s scroll wheel specified by `theEvent`.

