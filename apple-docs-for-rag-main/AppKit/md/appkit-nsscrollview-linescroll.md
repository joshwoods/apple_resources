

- AppKit
- NSScrollView
-  lineScroll 

Instance Property

# lineScroll

The scroll view’s line by line scroll amount.

macOS

``` source
@MainActor
var lineScroll: CGFloat { get set }
```

## Discussion

The value of this property is the amount by which the scroll view scrolls itself when scrolling line by line, expressed in the content view’s coordinate system. This value is used when the user clicks the scroll arrows without holding down a modifier key. When displaying text in a scroll view, for example, you might set this value to the height of a single line of text in the default font. As part of its implementation, this property accesses verticalLineScroll.

Note that a scroll view can have two different line scroll amounts: verticalLineScroll and horizontalLineScroll. Set this property only if you can be sure they’re both the same; setting this property sets both verticalLineScroll and horizontalLineScroll to the same value.

## See Also

### Setting Scrolling Behavior

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

func scrollWheel(with: NSEvent)

Scrolls the receiver up or down, in response to the user moving the mouse’s scroll wheel specified by `theEvent`.

