

- Swift
- Duration
- Duration.UnitsFormatStyle
-  Duration.UnitsFormatStyle.Unit 

Structure

# Duration.UnitsFormatStyle.Unit

A unit to use in formatting a duration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Unit
```

## Overview

Supported units range from hours to nanoseconds. Use these with the `allowed` parameter of the Duration.UnitsFormatStyle initializers to specify which units to use in a formatted string.

## Topics

### Duration units

static var hours: Duration.UnitsFormatStyle.Unit

The hours unit, used for formatting a duration.

static var minutes: Duration.UnitsFormatStyle.Unit

The minutes unit, used for formatting a duration.

static var seconds: Duration.UnitsFormatStyle.Unit

The seconds unit, used for formatting a duration.

static var milliseconds: Duration.UnitsFormatStyle.Unit

The milliseconds unit, used for formatting a duration.

static var microseconds: Duration.UnitsFormatStyle.Unit

The microseconds unit, used for formatting a duration.

static var nanoseconds: Duration.UnitsFormatStyle.Unit

The nanoseconds unit, used for formatting a duration.

### Type Properties

static var days: Duration.UnitsFormatStyle.Unit

The unit for days. One day is always 86400 seconds.

static var weeks: Duration.UnitsFormatStyle.Unit

The unit for weeks. One week is always 604800 seconds.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Working with units

var allowedUnits: Set&lt;Duration.UnitsFormatStyle.Unit>

The units that may be included in the output string.

var maximumUnitCount: Int?

The maximum number of time units to include in the output string.

var valueLengthLimits: Range&lt;Int>?

The padding or truncating behavior of the unit value.

