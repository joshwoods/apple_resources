

- Foundation
- NSTextCheckingResult
-  dateCheckingResult(range:date:) 

Type Method

# dateCheckingResult(range:date:)

Creates and returns a text checking result with the specified date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func dateCheckingResult(
    range: NSRange,
    date: Date
) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

`date`  

The detected date.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of date.

## See Also

### Text Checking Results for Dates and Times

class func dateCheckingResult(range: NSRange, date: Date, timeZone: TimeZone, duration: TimeInterval) -> NSTextCheckingResult

Creates and returns a text checking result with the specified date, time zone, and duration.

var date: Date?

The date component of a type checking result.

var duration: TimeInterval

The duration component of a type checking result.

var timeZone: TimeZone?

The time zone component of a type checking result.

