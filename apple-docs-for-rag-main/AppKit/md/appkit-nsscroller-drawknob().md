

- AppKit
- NSScroller
-  drawKnob() 

Instance Method

# drawKnob()

Draws the knob.

macOS

``` source
@MainActor
func drawKnob()
```

## Discussion

You should never need to invoke this method directly, but may wish to override it to customize the appearance of the knob.

## See Also

### Related Documentation

func rect(for: NSScroller.Part) -> NSRect

Returns the rectangle occupied by `aPart`, which for this method is interpreted literally rather than as an indicator of scrolling direction.

### Drawing Scroller Parts

func drawArrow(NSScroller.Arrow, highlight: Bool)

Draws the scroll button indicated by `arrow`, which is either `NSScrollerIncrementArrow` (the down or right scroll button) or `NSScrollerDecrementArrow` (up or left).

Deprecated

func drawKnobSlot(in: NSRect, highlight: Bool)

Draws the portion of the scroller’s track, possibly including the line increment and decrement arrow buttons, that falls in the given rectangle.

func highlight(Bool)

Highlights or unhighlights the scroll button the user clicked.

Deprecated

