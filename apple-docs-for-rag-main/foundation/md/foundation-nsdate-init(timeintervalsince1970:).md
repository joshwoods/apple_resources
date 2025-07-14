

- Foundation
- NSDate
-  init(timeIntervalSince1970:) 

Initializer

# init(timeIntervalSince1970:)

Returns a date object initialized relative to 00:00:00 UTC on 1 January 1970 by a given number of seconds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(timeIntervalSince1970 secs: TimeInterval)
```

## Parameters 

`secs`  

The number of seconds from the reference date (00:00:00 UTC on 1 January 1970) for the new date. Use a negative argument to specify a date and time before the reference date.

## Return Value

An `NSDate` object set to `seconds` seconds from the reference date.

## Discussion

This method is useful for creating `NSDate` objects from time_t values returned by BSD system functions.

## See Also

### Initializing a Date

init()

Returns a date object initialized to the current date and time.

convenience init(timeIntervalSinceNow: TimeInterval)

Returns a date object initialized relative to the current date and time by a given number of seconds.

convenience init(timeInterval: TimeInterval, sinceDate: Date)

Returns a date object initialized relative to another given date by a given number of seconds.

init(timeIntervalSinceReferenceDate: TimeInterval)

Returns a date object initialized relative to 00:00:00 UTC on 1 January 2001 by a given number of seconds.

init?(coder: NSCoder)

Returns a date object initialized from data in the given unarchiver.

