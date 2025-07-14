

- AppKit
- NSSliderCell
-  numberOfTickMarks 

Instance Property

# numberOfTickMarks

The number of tick marks associated with the slider, including the tick marks assigned to the minimum and maximum values.

macOS

``` source
@MainActor
var numberOfTickMarks: Int { get set }
```

## Discussion

By default, this value is 0, and no tick marks appear. The number of tick marks assigned to a slider, along with the slider’s minimum and maximum values, determines the values associated with the tick marks.

## See Also

### Managing Tick Marks

var allowsTickMarkValuesOnly: Bool

A Boolean value indicating whether the receiver fixes its values to those values represented by its tick marks.

func closestTickMarkValue(toValue: Double) -> Double

Returns the value of the tick mark closest to the specified value.

func indexOfTickMark(at: NSPoint) -> Int

Returns the index of the tick mark closest to the location of the slider represented by the specified point.

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark at the specified index.

var tickMarkPosition: NSSlider.TickMarkPosition

The position of the tick marks relative to the receiver.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at the specified index.

