

- AppKit
- NSSlider
-  tickMarkPosition 

Instance Property

# tickMarkPosition

Determines where the slider’s tick marks are displayed.

macOS

``` source
@MainActor
var tickMarkPosition: NSSlider.TickMarkPosition { get set }
```

## Discussion

For horizontal sliders, use NSSlider.TickMarkPosition.below and NSSlider.TickMarkPosition.above. For vertical sliders, use leading, and trailing. The default positions are `below` for horizontal and `leading` for vertical. This property has no effect if numberOfTickMarks is `0`, or if the slider is circular. In its implementation of this property, the receiving `NSSlider` instance invokes the method of the same name of its `NSSliderCell` instance.

## See Also

### Managing Tick Marks

var allowsTickMarkValuesOnly: Bool

A Boolean value that indicates whether the slider fixes its values to those values represented by its tick marks.

func closestTickMarkValue(toValue: Double) -> Double

Returns the value of the tick mark closest to the specified value.

func indexOfTickMark(at: NSPoint) -> Int

Returns the index of the tick mark closest to the location of the slider represented by the given point.

var numberOfTickMarks: Int

The number of tick marks associated with the slider.

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark at the given index.

enum TickMarkPosition

The position where a linear slider’s tick marks appear (above, below, leading, or trailing).

func tickMarkValue(at: Int) -> Double

Returns the slider’s value represented by the tick mark at the specified index.

