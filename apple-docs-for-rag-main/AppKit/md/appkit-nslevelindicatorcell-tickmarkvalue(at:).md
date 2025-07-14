

- AppKit
- NSLevelIndicatorCell
-  tickMarkValue(at:) 

Instance Method

# tickMarkValue(at:)

Returns the receiver’s value represented by the tick mark at index (the minimum-value tick mark has an index of 0).

macOS

``` source
@MainActor
func tickMarkValue(at index: Int) -> Double
```

## See Also

### Managing Tick Marks

var tickMarkPosition: NSSlider.TickMarkPosition

The placement of tick marks on the level indicator control.

var numberOfTickMarks: Int

The number of tick marks displayed by the control.

var numberOfMajorTickMarks: Int

The number of major tick marks displayed by the control.

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark identified by `index` (the minimum-value tick mark is at index 0).

