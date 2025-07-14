

- AppKit
- NSLevelIndicator
-  tickMarkPosition 

Instance Property

# tickMarkPosition

Determines how the receiver’s tick marks are aligned with it.

macOS

``` source
@MainActor
var tickMarkPosition: NSSlider.TickMarkPosition { get set }
```

## Discussion

The default alignments are `NSTickMarkBelow` and `NSTickMarkLeft`. This property has no effect if no tick marks have been assigned (that is, numberOfTickMarks returns 0).

## See Also

### Managing Tick Marks and Style

var numberOfTickMarks: Int

The number of tick marks associated with the receiver.

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

