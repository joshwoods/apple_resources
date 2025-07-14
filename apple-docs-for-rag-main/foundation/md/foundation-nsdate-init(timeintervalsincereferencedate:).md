

- Foundation
- NSDate
-  init(timeIntervalSinceReferenceDate:) 

Initializer

# init(timeIntervalSinceReferenceDate:)

Returns a date object initialized relative to 00:00:00 UTC on 1 January 2001 by a given number of seconds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(timeIntervalSinceReferenceDate ti: TimeInterval)
```

## Parameters 

`ti`  

The number of seconds to add to the reference date (00:00:00 UTC on 1 January 2001). A negative value means the receiver will be earlier than the reference date.

## Return Value

An `NSDate` object initialized relative to the absolute reference date by `ti` seconds.

## Discussion

This method is a designated initializer for the `NSDate` class and is declared primarily for the use of subclasses of `NSDate`. When you subclass `NSDate` to create a concrete date class, you must override this method.

## See Also

### Initializing a Date

init()

Returns a date object initialized to the current date and time.

convenience init(timeIntervalSinceNow: TimeInterval)

Returns a date object initialized relative to the current date and time by a given number of seconds.

convenience init(timeInterval: TimeInterval, sinceDate: Date)

Returns a date object initialized relative to another given date by a given number of seconds.

convenience init(timeIntervalSince1970: TimeInterval)

Returns a date object initialized relative to 00:00:00 UTC on 1 January 1970 by a given number of seconds.

init?(coder: NSCoder)

Returns a date object initialized from data in the given unarchiver.

