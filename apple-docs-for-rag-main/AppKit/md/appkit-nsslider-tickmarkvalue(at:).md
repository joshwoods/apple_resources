

- AppKit
- NSSlider
-  tickMarkValue(at:) 

Instance Method

# tickMarkValue(at:)

Returns the slider’s value represented by the tick mark at the specified index.

macOS

``` source
@MainActor
func tickMarkValue(at index: Int) -> Double
```

## Parameters 

`index`  

The index of the tick mark for which to return the value. The minimum-value tick mark has an index of `0`.

## Return Value

The value of the specified tick mark.

## Discussion

In its implementation of this method, the receiving `NSSlider` instance invokes the method of the same name of its `NSSliderCell` instance.

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

var tickMarkPosition: NSSlider.TickMarkPosition

Determines where the slider’s tick marks are displayed.

enum TickMarkPosition

The position where a linear slider’s tick marks appear (above, below, leading, or trailing).

