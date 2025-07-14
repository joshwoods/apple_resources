

- AppKit
- NSSliderCell
-  barRect(flipped:) 

Instance Method

# barRect(flipped:)

Returns the rectangle in which the bar is drawn.

macOS 10.9+

``` source
@MainActor
func barRect(flipped: Bool) -> NSRect
```

## Parameters 

`flipped`  

true if the coordinate system of the associated `NSSlider` or `NSMatrix` is flipped; otherwise false. You can determine whether this is the case by sending the `NSView` message isFlipped message to the `NSMatrix` or `NSSlider`.

## Return Value

The rectangle in which the bar is drawn, specified in the coordinate system of the `NSSlider` or `NSMatrix` with which the receiver is associated. The bar doesn’t include the slider’s bezel or knob.

## Discussion

You can override this method if custom bar artwork requires specific dimensions.

## See Also

### Displaying the Cell

func drawTickMarks()

Draws the slider’s tick marks.

func knobRect(flipped: Bool) -> NSRect

Returns the rectangle in which the slider knob is drawn.

func drawBar(inside: NSRect, flipped: Bool)

Draws the slider’s bar—but not its bezel or knob—inside the specified rectangle.

func drawKnob()

Calculates the rectangle in which the knob should be drawn, then calls drawKnob(_:) to actually draw the knob.

func drawKnob(NSRect)

Draws the slider knob in the given rectangle.

