

- AppKit
- NSSlider
-  NSSlider.TickMarkPosition 

Enumeration

# NSSlider.TickMarkPosition

The position where a linear slider’s tick marks appear (above, below, leading, or trailing).

macOS

``` source
enum TickMarkPosition
```

## Overview

Use these constants for setting tickMarkPosition.

## Topics

### Configuring Horizontal Sliders

case below

A constant indicating that tick marks are displayed below the slider.

case above

A constant indicating that tick marks are displayed above the slider.

### Configuring Vertical Sliders

static var leading: NSSlider.TickMarkPosition

A constant indicating that tick marks are displayed on the leading side of the slider.

static var trailing: NSSlider.TickMarkPosition

A constant indicating that tick marks are displayed on the trailing side of the slider.

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

### Managing Tick Marks

var allowsTickMarkValuesOnly: Bool

A Boolean value that indicates whether the slider fixes its values to those values represented by its tick marks.

func closestTickMarkValue(toValue: Double) -> Double

Returns the value of the tick mark closest to the specified value.

func indexOfTickMark(at: NSPoint) -> Int

Returns the index of the tick mark closest to the location of the slider represented by the given point.

var numberOfTickMarks: Int

The number of tick marks associated with the slider.

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark at the given index.

var tickMarkPosition: NSSlider.TickMarkPosition

Determines where the slider’s tick marks are displayed.

func tickMarkValue(at: Int) -> Double

Returns the slider’s value represented by the tick mark at the specified index.

