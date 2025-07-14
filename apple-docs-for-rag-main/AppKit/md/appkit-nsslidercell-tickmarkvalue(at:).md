

- AppKit
- NSSliderCell
-  tickMarkValue(at:) 

Instance Method

# tickMarkValue(at:)

Returns the receiver’s value represented by the tick mark at the specified index.

macOS

``` source
@MainActor
func tickMarkValue(at index: Int) -> Double
```

## Parameters 

`index`  

The index of the tick mark for which to retrieve the value. The minimum-value tick mark has an index of 0.

## Return Value

The value represented by the specified tick mark.

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

var tickMarkPosition: NSSlider.TickMarkPosition

The position of the tick marks relative to the receiver.

