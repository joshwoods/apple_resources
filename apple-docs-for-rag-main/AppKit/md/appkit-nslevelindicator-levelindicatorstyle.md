

- AppKit
- NSLevelIndicator
-  levelIndicatorStyle 

Instance Property

# levelIndicatorStyle

The appearance of the indicator.

macOS 10.10+

``` source
@MainActor
var levelIndicatorStyle: NSLevelIndicator.Style { get set }
```

## Discussion

See NSLevelIndicator.Style for possible styles.

## See Also

### Managing Tick Marks and Style

var tickMarkPosition: NSSlider.TickMarkPosition

Determines how the receiver’s tick marks are aligned with it.

var numberOfTickMarks: Int

The number of tick marks associated with the receiver.

var numberOfMajorTickMarks: Int

The number of major tick marks associated with the receiver.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at the specified index (the minimum-value tick mark has an index of 0).

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark identified by the specified index (the minimum-value tick mark is at index 0).

enum Style

Constants that specify a level indicator’s appearance.

