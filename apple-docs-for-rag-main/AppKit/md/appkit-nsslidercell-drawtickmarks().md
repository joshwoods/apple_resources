

- AppKit
- NSSliderCell
-  drawTickMarks() 

Instance Method

# drawTickMarks()

Draws the slider’s tick marks.

macOS 10.9+

``` source
@MainActor
func drawTickMarks()
```

## Discussion

You should not call this method explicitly. It’s included so you can override it in a subclass and draw custom tick marks.

## See Also

### Displaying the Cell

func barRect(flipped: Bool) -> NSRect

Returns the rectangle in which the bar is drawn.

func knobRect(flipped: Bool) -> NSRect

Returns the rectangle in which the slider knob is drawn.

func drawBar(inside: NSRect, flipped: Bool)

Draws the slider’s bar—but not its bezel or knob—inside the specified rectangle.

func drawKnob()

Calculates the rectangle in which the knob should be drawn, then calls drawKnob(_:) to actually draw the knob.

func drawKnob(NSRect)

Draws the slider knob in the given rectangle.

