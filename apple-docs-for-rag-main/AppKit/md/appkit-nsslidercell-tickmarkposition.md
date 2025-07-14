

- AppKit
- NSSliderCell
-  tickMarkPosition 

Instance Property

# tickMarkPosition

The position of the tick marks relative to the receiver.

macOS

``` source
@MainActor
var tickMarkPosition: NSSlider.TickMarkPosition { get set }
```

## Discussion

The value of this property is a constant indicating the position of the tick marks. Possible values are described in NSSlider.TickMarkPosition. The default alignments are `NSTickMarkBelow` and `NSTickMarkLeft`. Setting this property has no effect if no tick marks have been assigned (that is, if numberOfTickMarks is 0).

## See Also

### Managing Tick Marks

var allowsTickMarkValuesOnly: Bool

A Boolean value indicating whether the receiver fixes its values to those values represented by its tick marks.

func closestTickMarkValue(toValue: Double) -> Double

Returns the value of the tick mark closest to the specified value.

func indexOfTickMark(at: NSPoint) -> Int

Returns the index of the tick mark closest to the location of the slider represented by the specified point.

var numberOfTickMarks: Int

The number of tick marks associated with the slider, including the tick marks assigned to the minimum and maximum values.

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark at the specified index.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at the specified index.

