

- AppKit
- NSLevelIndicator
-  tickMarkValue(at:) 

Instance Method

# tickMarkValue(at:)

Returns the receiver’s value represented by the tick mark at the specified index (the minimum-value tick mark has an index of 0).

macOS

``` source
@MainActor
func tickMarkValue(at index: Int) -> Double
```

## See Also

### Managing Tick Marks and Style

var tickMarkPosition: NSSlider.TickMarkPosition

Determines how the receiver’s tick marks are aligned with it.

var numberOfTickMarks: Int

The number of tick marks associated with the receiver.

var numberOfMajorTickMarks: Int

The number of major tick marks associated with the receiver.

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark identified by the specified index (the minimum-value tick mark is at index 0).

var levelIndicatorStyle: NSLevelIndicator.Style

The appearance of the indicator.

enum Style

Constants that specify a level indicator’s appearance.

