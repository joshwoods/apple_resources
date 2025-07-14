

- Swift
- Duration
- Duration.TimeFormatStyle
- Duration.TimeFormatStyle.Pattern
-  minuteSecond(padMinuteToLength:fractionalSecondsLength:roundFractionalSeconds:) 

Type Method

# minuteSecond(padMinuteToLength:fractionalSecondsLength:roundFractionalSeconds:)

Returns a pattern to format a duration with minutes and seconds only, with the given unit configurations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func minuteSecond(
    padMinuteToLength: Int,
    fractionalSecondsLength: Int = 0,
    roundFractionalSeconds: FloatingPointRoundingRule = .toNearestOrEven
) -> Duration.TimeFormatStyle.Pattern
```

## Parameters 

`padMinuteToLength`  

Padding for the minute field. For example, setting this value to `2` formats five minutes as `05:00` in the `en_US` locale.

`fractionalSecondsLength`  

The length of the fractional seconds. For example, setting this value to `2` formats five minutes as `5:00.00` in the `en_US` locale.

`roundFractionalSeconds`  

The rule to use for rounding the seconds value, given the remaining fractional seconds value. Use one of the cases from the FloatingPointRoundingRule enumeration.

## Return Value

A Duration.TimeFormatStyle.Pattern that formats a duration with minutes and seconds, using the given unit configurations.

## See Also

### Creating a pattern

static func hourMinute(padHourToLength: Int, roundSeconds: FloatingPointRoundingRule) -> Duration.TimeFormatStyle.Pattern

Returns a pattern to format a duration with hours and minutes only, with the given unit configurations.

static func hourMinuteSecond(padHourToLength: Int, fractionalSecondsLength: Int, roundFractionalSeconds: FloatingPointRoundingRule) -> Duration.TimeFormatStyle.Pattern

Returns a pattern to format a duration with hours, minutes, and seconds, with the given unit configurations.

