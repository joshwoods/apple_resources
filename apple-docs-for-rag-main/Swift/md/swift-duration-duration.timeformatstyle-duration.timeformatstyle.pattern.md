

- Swift
- Duration
- Duration.TimeFormatStyle
-  Duration.TimeFormatStyle.Pattern 

Structure

# Duration.TimeFormatStyle.Pattern

The units — including hours, minutes, or seconds — and the configuration of those units, used to format a duration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Pattern
```

## Overview

Use a pattern when initializing a Duration.TimeFormatStyle, or creating a time format style from the convenience method `Swift/Duration/TimeFormatStyle/time(pattern:)`.

Use the type properties hourMinute, hourMinuteSecond, or minuteSecond to create patterns with default behavior. To customize how a pattern handles zero-padding and fractional parts, use one of the type methods that take these customizations as parameters.

## Topics

### Creating a pattern

static func hourMinute(padHourToLength: Int, roundSeconds: FloatingPointRoundingRule) -> Duration.TimeFormatStyle.Pattern

Returns a pattern to format a duration with hours and minutes only, with the given unit configurations.

static func hourMinuteSecond(padHourToLength: Int, fractionalSecondsLength: Int, roundFractionalSeconds: FloatingPointRoundingRule) -> Duration.TimeFormatStyle.Pattern

Returns a pattern to format a duration with hours, minutes, and seconds, with the given unit configurations.

static func minuteSecond(padMinuteToLength: Int, fractionalSecondsLength: Int, roundFractionalSeconds: FloatingPointRoundingRule) -> Duration.TimeFormatStyle.Pattern

Returns a pattern to format a duration with minutes and seconds only, with the given unit configurations.

### Using common patterns

static var hourMinute: Duration.TimeFormatStyle.Pattern

A pattern to format a duration with hours and minutes only, with default padding and rounding behavior.

static var hourMinuteSecond: Duration.TimeFormatStyle.Pattern

A pattern to format a duration with hours, minutes, and seconds, with default padding and rounding behavior.

static var minuteSecond: Duration.TimeFormatStyle.Pattern

A pattern to format a duration with minutes and seconds only, with default padding and rounding behavior.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a time format style

init(pattern: Duration.TimeFormatStyle.Pattern, locale: Locale)

Creates a time format style using the provided pattern and optional locale.

