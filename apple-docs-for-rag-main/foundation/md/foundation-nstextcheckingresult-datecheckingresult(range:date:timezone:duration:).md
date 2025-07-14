

- Foundation
- NSTextCheckingResult
-  dateCheckingResult(range:date:timeZone:duration:) 

Type Method

# dateCheckingResult(range:date:timeZone:duration:)

Creates and returns a text checking result with the specified date, time zone, and duration.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func dateCheckingResult(
    range: NSRange,
    date: Date,
    timeZone: TimeZone,
    duration: TimeInterval
) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

`date`  

The detected date.

`timeZone`  

The detected time zone.

`duration`  

The detected duration.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of date.

## See Also

### Text Checking Results for Dates and Times

class func dateCheckingResult(range: NSRange, date: Date) -> NSTextCheckingResult

Creates and returns a text checking result with the specified date.

var date: Date?

The date component of a type checking result.

var duration: TimeInterval

The duration component of a type checking result.

var timeZone: TimeZone?

The time zone component of a type checking result.

