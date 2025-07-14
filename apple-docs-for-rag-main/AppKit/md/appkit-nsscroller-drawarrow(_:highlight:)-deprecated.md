

- AppKit
- NSScroller
-  drawArrow(\_:highlight:) Deprecated

Instance Method

# drawArrow(\_:highlight:)

Draws the scroll button indicated by `arrow`, which is either `NSScrollerIncrementArrow` (the down or right scroll button) or `NSScrollerDecrementArrow` (up or left).

macOS 10.0–10.14Deprecated

``` source
@MainActor
func drawArrow(
    _ whichArrow: NSScroller.Arrow,
    highlight flag: Bool
)
```

Deprecated

Scrollers don't have arrows as of 10.7

## Discussion

If `flag` is true, the button is drawn highlighted; otherwise it’s drawn normally. You should never need to invoke this method directly, but may wish to override it to customize the appearance of scroll buttons.

Note

The drawArrow(_:highlight:) method is not invoked in macOS 10.7 and later.

## See Also

### Related Documentation

func rect(for: NSScroller.Part) -> NSRect

Returns the rectangle occupied by `aPart`, which for this method is interpreted literally rather than as an indicator of scrolling direction.

### Drawing Scroller Parts

func drawKnobSlot(in: NSRect, highlight: Bool)

Draws the portion of the scroller’s track, possibly including the line increment and decrement arrow buttons, that falls in the given rectangle.

func drawKnob()

Draws the knob.

func highlight(Bool)

Highlights or unhighlights the scroll button the user clicked.

Deprecated

