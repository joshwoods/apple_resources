

- AppKit
- NSLevelIndicator
-  numberOfTickMarks 

Instance Property

# numberOfTickMarks

The number of tick marks associated with the receiver.

macOS

``` source
@MainActor
var numberOfTickMarks: Int { get set }
```

## Discussion

By default, this value is 0, and no tick marks appear. The number of tick marks assigned to a slider, along with the slider’s minimum and maximum values, determines the values associated with the tick marks.

## See Also

### Managing Tick Marks and Style

var tickMarkPosition: NSSlider.TickMarkPosition

Determines how the receiver’s tick marks are aligned with it.

var numberOfMajorTickMarks: Int

The number of major tick marks associated with the receiver.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at the specified index (the minimum-value tick mark has an index of 0).

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark identified by the specified index (the minimum-value tick mark is at index 0).

var levelIndicatorStyle: NSLevelIndicator.Style

The appearance of the indicator.

enum Style

Constants that specify a level indicator’s appearance.

