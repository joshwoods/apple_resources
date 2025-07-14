

- AppKit
- NSScroller
-  highlight(\_:) Deprecated

Instance Method

# highlight(\_:)

Highlights or unhighlights the scroll button the user clicked.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func highlight(_ flag: Bool)
```

Deprecated

Has had no effect since 10.7

## Discussion

The receiver invokes this method while tracking the mouse; you should not invoke it directly. If `flag` is true, the appropriate part is drawn highlighted; otherwise it’s drawn normally.

### Special Considerations

This method has no effect in macOS 10.7 and later.

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

func drawKnob()

Draws the knob.

