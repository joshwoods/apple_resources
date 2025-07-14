

- AppKit
- NSSlider
-  rectOfTickMark(at:) 

Instance Method

# rectOfTickMark(at:)

Returns the bounding rectangle of the tick mark at the given index.

macOS

``` source
@MainActor
func rectOfTickMark(at index: Int) -> NSRect
```

## Parameters 

`index`  

The index of the tick mark for which to retrieve the bounds. The minimum-value tick mark is at index `0`.

## Return Value

The bounding rectangle of the specified tick mark.

## Discussion

If no tick mark is associated with `index`, the method raises `NSRangeException`. In its implementation of this method, the receiving `NSSlider` instance invokes the method of the same name of its NSSliderCell instance.

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

var tickMarkPosition: NSSlider.TickMarkPosition

Determines where the slider’s tick marks are displayed.

enum TickMarkPosition

The position where a linear slider’s tick marks appear (above, below, leading, or trailing).

func tickMarkValue(at: Int) -> Double

Returns the slider’s value represented by the tick mark at the specified index.

