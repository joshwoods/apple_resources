

- AppKit
- NSSliderCell
-  allowsTickMarkValuesOnly 

Instance Property

# allowsTickMarkValuesOnly

A Boolean value indicating whether the receiver fixes its values to those values represented by its tick marks.

macOS

``` source
@MainActor
var allowsTickMarkValuesOnly: Bool { get set }
```

## Discussion

The value of this property is true if the slider’s values are limited to those values represented by tick marks; otherwise, false. For example, if you specify true for a slider that has a minimum value of 0, a maximum value of 100, and five markers, the allowable values are 0, 25, 50, 75, and 100. When users move the slider’s knob, it jumps to the tick mark nearest the pointer when the mouse button is released. Setting this property has no effect if the slider has no tick marks.

## See Also

### Managing Tick Marks

func closestTickMarkValue(toValue: Double) -> Double

Returns the value of the tick mark closest to the specified value.

func indexOfTickMark(at: NSPoint) -> Int

Returns the index of the tick mark closest to the location of the slider represented by the specified point.

var numberOfTickMarks: Int

The number of tick marks associated with the slider, including the tick marks assigned to the minimum and maximum values.

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark at the specified index.

var tickMarkPosition: NSSlider.TickMarkPosition

The position of the tick marks relative to the receiver.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at the specified index.

