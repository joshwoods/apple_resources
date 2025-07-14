

- AppKit
- NSLevelIndicator
-  NSLevelIndicator.Style 

Enumeration

# NSLevelIndicator.Style

Constants that specify a level indicator’s appearance.

macOS

``` source
enum Style
```

## Topics

### Level Indicator Styles

case relevancy

A style that indicates the relevancy of an item, such as a search result.

case continuousCapacity

A style that indicates the capacity of something, such as how much data is on a hard disk.

case discreteCapacity

A style that displays discrete segments that indicate the capacity of something, such as an audio level.

case rating

A style that indicates a rank, such as a star ranking display.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var levelIndicatorStyle: NSLevelIndicator.Style

The appearance of the indicator.

