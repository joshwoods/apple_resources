

- Foundation
- ISO8601DateFormatter
- ISO8601DateFormatter.Options
-  withDay 

Type Property

# withDay

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static var withDay: ISO8601DateFormatter.Options { get }
```

## Discussion

The date representation includes the day. The format for day is inferred based on provided options:

- If withMonth is specified, `dd` is used.

- If withWeekOfYear is specified, `ee` is used.

- Otherwise, `DDD` is used.

## See Also

### Constants

static var withYear: ISO8601DateFormatter.Options

static var withMonth: ISO8601DateFormatter.Options

static var withWeekOfYear: ISO8601DateFormatter.Options

static var withTime: ISO8601DateFormatter.Options

static var withTimeZone: ISO8601DateFormatter.Options

static var withSpaceBetweenDateAndTime: ISO8601DateFormatter.Options

static var withDashSeparatorInDate: ISO8601DateFormatter.Options

static var withColonSeparatorInTime: ISO8601DateFormatter.Options

static var withColonSeparatorInTimeZone: ISO8601DateFormatter.Options

static var withFullDate: ISO8601DateFormatter.Options

static var withFullTime: ISO8601DateFormatter.Options

static var withInternetDateTime: ISO8601DateFormatter.Options

static var withYear: ISO8601DateFormatter.Options

static var withMonth: ISO8601DateFormatter.Options

static var withWeekOfYear: ISO8601DateFormatter.Options

