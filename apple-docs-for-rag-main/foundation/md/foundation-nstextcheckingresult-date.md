

- Foundation
- NSTextCheckingResult
-  date 

Instance Property

# date

The date component of a type checking result.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var date: Date? { get }
```

## See Also

### Text Checking Results for Dates and Times

class func dateCheckingResult(range: NSRange, date: Date) -> NSTextCheckingResult

Creates and returns a text checking result with the specified date.

class func dateCheckingResult(range: NSRange, date: Date, timeZone: TimeZone, duration: TimeInterval) -> NSTextCheckingResult

Creates and returns a text checking result with the specified date, time zone, and duration.

var duration: TimeInterval

The duration component of a type checking result.

var timeZone: TimeZone?

The time zone component of a type checking result.

