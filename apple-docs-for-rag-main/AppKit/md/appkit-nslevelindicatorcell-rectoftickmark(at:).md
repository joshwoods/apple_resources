

- AppKit
- NSLevelIndicatorCell
-  rectOfTickMark(at:) 

Instance Method

# rectOfTickMark(at:)

Returns the bounding rectangle of the tick mark identified by `index` (the minimum-value tick mark is at index 0).

macOS

``` source
@MainActor
func rectOfTickMark(at index: Int) -> NSRect
```

## Discussion

If no tick mark is associated with `index`, the method raises a `NSRangeException`.

## See Also

### Managing Tick Marks

var tickMarkPosition: NSSlider.TickMarkPosition

The placement of tick marks on the level indicator control.

var numberOfTickMarks: Int

The number of tick marks displayed by the control.

var numberOfMajorTickMarks: Int

The number of major tick marks displayed by the control.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at index (the minimum-value tick mark has an index of 0).

