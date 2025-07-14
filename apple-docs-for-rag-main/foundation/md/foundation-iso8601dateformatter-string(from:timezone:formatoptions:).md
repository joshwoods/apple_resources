

- Foundation
- ISO8601DateFormatter
-  string(from:timeZone:formatOptions:) 

Type Method

# string(from:timeZone:formatOptions:)

Creates a representation of the specified date with a given time zone and format options.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class func string(
    from date: Date,
    timeZone: TimeZone,
    formatOptions: ISO8601DateFormatter.Options = []
) -> String
```

## Parameters 

`date`  

The date to be represented.

`timeZone`  

The time zone used.

`formatOptions`  

The options used. For possible values, see ISO8601DateFormatter.Options.

## Return Value

A user-readable string representing the date.

## Discussion

This method uses a date formatter configured with the specified time zone and format options. The following code examples produce the same string value:

- Swift
- Objective-C

```
let date = Date()
var string: String

let formatter = ISO8601DateFormatter()
string = formatter.string(from: date)

if let GMT = TimeZone(abbreviation: "GMT") {
    let options: ISO8601DateFormatter.Options = [.withInternetDateTime, .withDashSeparatorInDate, .withColonSeparatorInTime, .withTimeZone]
    string = ISO8601DateFormatter.string(from: date, timeZone: GMT, formatOptions: options)
}
```

```
NSDate *date = [NSDate date];
NSString *string;

NSISO8601DateFormatter *formatter = [[NSISO8601DateFormatter alloc] init];
string = [formatter stringFromDate:date];

NSTimeZone *GMT = [NSTimeZone timeZoneWithAbbreviation: @"GMT"];
NSISO8601DateFormatOptions options = NSISO8601DateFormatWithInternetDateTime | NSISO8601DateFormatWithDashSeparatorInDate | NSISO8601DateFormatWithColonSeparatorInTime | NSISO8601DateFormatWithTimeZone;
string = [NSISO8601DateFormatter stringFromDate:date timeZone:GMT formatOptions:options];
```

## See Also

### Converting ISO 8601 Dates

func string(from: Date) -> String

Creates and returns an ISO 8601 formatted string representation of the specified date.

func date(from: String) -> Date?

Creates and returns a date object from the specified ISO 8601 formatted string representation.

