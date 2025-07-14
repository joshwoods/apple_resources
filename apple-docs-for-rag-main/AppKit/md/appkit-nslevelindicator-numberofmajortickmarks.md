

- AppKit
- NSLevelIndicator
-  numberOfMajorTickMarks 

Instance Property

# numberOfMajorTickMarks

The number of major tick marks associated with the receiver.

macOS

``` source
@MainActor
var numberOfMajorTickMarks: Int { get set }
```

## Discussion

The number of major tick marks must be less than or equal to the number of tick marks returned by numberOfTickMarks. For example, if the number of tick marks is 11 and you specify 3 major tick marks, the resulting level indicator will display 3 major tick marks alternating with 8 minor tick marks, as in the example shown in NSLevelIndicator.

## See Also

### Managing Tick Marks and Style

var tickMarkPosition: NSSlider.TickMarkPosition

Determines how the receiver’s tick marks are aligned with it.

var numberOfTickMarks: Int

The number of tick marks associated with the receiver.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at the specified index (the minimum-value tick mark has an index of 0).

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark identified by the specified index (the minimum-value tick mark is at index 0).

var levelIndicatorStyle: NSLevelIndicator.Style

The appearance of the indicator.

enum Style

Constants that specify a level indicator’s appearance.

