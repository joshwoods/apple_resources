

- AppKit
- NSSliderCell
-  indexOfTickMark(at:) 

Instance Method

# indexOfTickMark(at:)

Returns the index of the tick mark closest to the location of the slider represented by the specified point.

macOS

``` source
@MainActor
func indexOfTickMark(at point: NSPoint) -> Int
```

## Parameters 

`point`  

The point representing the slider location.

## Return Value

The index of the tick mark closest to the specified location.

## Discussion

If `point` is not within the bounding rectangle (plus an extra pixel of space) of any tick mark, the method returns `NSNotFound`. This method calls rectOfTickMark(at:) for each tick mark on the slider until it finds a tick mark containing `point`.

## See Also

### Managing Tick Marks

var allowsTickMarkValuesOnly: Bool

A Boolean value indicating whether the receiver fixes its values to those values represented by its tick marks.

func closestTickMarkValue(toValue: Double) -> Double

Returns the value of the tick mark closest to the specified value.

var numberOfTickMarks: Int

The number of tick marks associated with the slider, including the tick marks assigned to the minimum and maximum values.

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark at the specified index.

var tickMarkPosition: NSSlider.TickMarkPosition

The position of the tick marks relative to the receiver.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at the specified index.

