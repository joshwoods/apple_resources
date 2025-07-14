

- AppKit
- NSSlider
-  closestTickMarkValue(toValue:) 

Instance Method

# closestTickMarkValue(toValue:)

Returns the value of the tick mark closest to the specified value.

macOS

``` source
@MainActor
func closestTickMarkValue(toValue value: Double) -> Double
```

## Parameters 

`value`  

The value for which to return the closest tick mark.

## Return Value

The value of the tick mark closest to `aValue`.

## Discussion

In its implementation of this method, the slider invokes the method of the same name of its `NSSliderCell` instance.

## See Also

### Managing Tick Marks

var allowsTickMarkValuesOnly: Bool

A Boolean value that indicates whether the slider fixes its values to those values represented by its tick marks.

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

func tickMarkValue(at: Int) -> Double

Returns the slider’s value represented by the tick mark at the specified index.

