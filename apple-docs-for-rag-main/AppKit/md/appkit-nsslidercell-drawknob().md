

- AppKit
- NSSliderCell
-  drawKnob() 

Instance Method

# drawKnob()

Calculates the rectangle in which the knob should be drawn, then calls drawKnob(_:) to actually draw the knob.

macOS

``` source
@MainActor
func drawKnob()
```

## Discussion

Before this message is sent, a `lockFocus` method must be sent to the cell’s control view.

You might call this method if you override one of the display methods belonging to `NSControl` or `NSCell`.

### Special Considerations

If you create a subclass of `NSSliderCell`, don’t override this method. Override drawKnob(_:) instead.

## See Also

### Displaying the Cell

func barRect(flipped: Bool) -> NSRect

Returns the rectangle in which the bar is drawn.

func drawTickMarks()

Draws the slider’s tick marks.

func knobRect(flipped: Bool) -> NSRect

Returns the rectangle in which the slider knob is drawn.

func drawBar(inside: NSRect, flipped: Bool)

Draws the slider’s bar—but not its bezel or knob—inside the specified rectangle.

func drawKnob(NSRect)

Draws the slider knob in the given rectangle.

