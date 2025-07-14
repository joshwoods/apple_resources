

- AppKit
- NSSliderCell
-  drawBar(inside:flipped:) 

Instance Method

# drawBar(inside:flipped:)

Draws the slider’s bar—but not its bezel or knob—inside the specified rectangle.

macOS

``` source
@MainActor
func drawBar(
    inside rect: NSRect,
    flipped: Bool
)
```

## Parameters 

`rect`  

The bounds of the slider’s bar, not of its interior rectangle.

`flipped`  

A Boolean value that indicates whether the cell’s control view—that is, the `NSSlider` or `NSMatrix` associated with the `NSSliderCell`—has a flipped coordinate system.

## Discussion

You should not call this method explicitly. It’s included so you can override it in a subclass.

## See Also

### Displaying the Cell

func barRect(flipped: Bool) -> NSRect

Returns the rectangle in which the bar is drawn.

func drawTickMarks()

Draws the slider’s tick marks.

func knobRect(flipped: Bool) -> NSRect

Returns the rectangle in which the slider knob is drawn.

func drawKnob()

Calculates the rectangle in which the knob should be drawn, then calls drawKnob(_:) to actually draw the knob.

func drawKnob(NSRect)

Draws the slider knob in the given rectangle.

