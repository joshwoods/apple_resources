

- AppKit
- NSScroller
-  drawKnobSlot(in:highlight:) 

Instance Method

# drawKnobSlot(in:highlight:)

Draws the portion of the scroller’s track, possibly including the line increment and decrement arrow buttons, that falls in the given rectangle.

macOS

``` source
@MainActor
func drawKnobSlot(
    in slotRect: NSRect,
    highlight flag: Bool
)
```

## Parameters 

`slotRect`  

The rectangle in which to draw the knob slot.

`flag`  

If `flag` is true, any scroll arrow button that falls within `slotRect` is drawn highlighted; otherwise it’s drawn normally.

## Discussion

Only one arrow button will be shown highlighted at a time, so you can expect this method to sometimes be invoked with a `slotRect` that encompasses only one arrow.

## See Also

### Drawing Scroller Parts

func drawArrow(NSScroller.Arrow, highlight: Bool)

Draws the scroll button indicated by `arrow`, which is either `NSScrollerIncrementArrow` (the down or right scroll button) or `NSScrollerDecrementArrow` (up or left).

Deprecated

func drawKnob()

Draws the knob.

func highlight(Bool)

Highlights or unhighlights the scroll button the user clicked.

Deprecated

