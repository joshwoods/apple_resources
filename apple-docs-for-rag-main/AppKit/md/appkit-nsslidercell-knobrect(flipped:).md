

- AppKit
- NSSliderCell
-  knobRect(flipped:) 

Instance Method

# knobRect(flipped:)

Returns the rectangle in which the slider knob is drawn.

macOS

``` source
@MainActor
func knobRect(flipped: Bool) -> NSRect
```

## Parameters 

`flipped`  

true if the coordinate system of the associated `NSSlider` or `NSMatrix` is flipped; otherwise false. You can determine whether this is the case by sending the `NSView` message isFlipped message to the `NSMatrix` or `NSSlider`.

## Return Value

The rectangle in which the knob is drawn, specified in the coordinate system of the `NSSlider` or `NSMatrix` with which the receiver is associated.

## Discussion

The knob rectangle depends on where in the slider the knob belongs—that is, it depends on the receiver’s minimum and maximum values and on the value the position of the knob will represent.

## See Also

### Displaying the Cell

func barRect(flipped: Bool) -> NSRect

Returns the rectangle in which the bar is drawn.

func drawTickMarks()

Draws the slider’s tick marks.

func drawBar(inside: NSRect, flipped: Bool)

Draws the slider’s bar—but not its bezel or knob—inside the specified rectangle.

func drawKnob()

Calculates the rectangle in which the knob should be drawn, then calls drawKnob(_:) to actually draw the knob.

func drawKnob(NSRect)

Draws the slider knob in the given rectangle.

