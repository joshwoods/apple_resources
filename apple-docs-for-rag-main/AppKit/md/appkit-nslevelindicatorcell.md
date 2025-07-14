

- AppKit
-  NSLevelIndicatorCell 

Class

# NSLevelIndicatorCell

`NSLevelIndicatorCell` is a subclass of NSActionCell that provides several level indicator display styles including: capacity, ranking and relevancy. The capacity style provides both continuous and discrete modes.

macOS

``` source
@MainActor
class NSLevelIndicatorCell
```

## Topics

### Initializing NSLevelIndicatorCell Objects

init(levelIndicatorStyle: NSLevelIndicator.Style)

Initializes the receiver with the style specified by `levelIndicatorStyle`.

### Configuring the Range of Values

var minValue: Double

The minimum value of the control.

var maxValue: Double

The maximum value of the control.

var levelIndicatorStyle: NSLevelIndicator.Style

The style of the level indicator control.

var warningValue: Double

The warning value of the level indicator control.

var criticalValue: Double

The critical value of the level indicator control.

### Managing Tick Marks

var tickMarkPosition: NSSlider.TickMarkPosition

The placement of tick marks on the level indicator control.

var numberOfTickMarks: Int

The number of tick marks displayed by the control.

var numberOfMajorTickMarks: Int

The number of major tick marks displayed by the control.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at index (the minimum-value tick mark has an index of 0).

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark identified by `index` (the minimum-value tick mark is at index 0).

### Constants

enum Style

Constants that specify a level indicator’s appearance.

## Relationships

### Inherits From

- NSActionCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

