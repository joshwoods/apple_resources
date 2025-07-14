

- AppKit
- NSSliderCell
-  drawKnob(\_:) 

Instance Method

# drawKnob(\_:)

Draws the slider knob in the given rectangle.

macOS

``` source
@MainActor
func drawKnob(_ knobRect: NSRect)
```

## Parameters 

`knobRect`  

The rectangle in which to draw the slider knob.

## Discussion

Before this message is sent, a lockFocus() message must be sent to the cell’s control view.

You should not call this method explicitly. It’s included so you can override it in a subclass.

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

func drawKnob()

Calculates the rectangle in which the knob should be drawn, then calls drawKnob(_:) to actually draw the knob.

