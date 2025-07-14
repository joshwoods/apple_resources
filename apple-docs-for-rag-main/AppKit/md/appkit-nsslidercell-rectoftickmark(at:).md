

- AppKit
- NSSliderCell
-  rectOfTickMark(at:) 

Instance Method

# rectOfTickMark(at:)

Returns the bounding rectangle of the tick mark at the specified index.

macOS

``` source
@MainActor
func rectOfTickMark(at index: Int) -> NSRect
```

## Parameters 

`index`  

The index of the tick mark for which to return the bounding rectangle. The minimum-value tick mark is at index 0.

## Return Value

The bounding rectangle of the specified tick mark.

## Discussion

If no tick mark is associated with `index`, the method raises `NSRangeException`.

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

var tickMarkPosition: NSSlider.TickMarkPosition

The position of the tick marks relative to the receiver.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at the specified index.

