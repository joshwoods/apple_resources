

- Foundation
- NSDate
-  init(timeInterval:sinceDate:) 

Initializer

# init(timeInterval:sinceDate:)

Returns a date object initialized relative to another given date by a given number of seconds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    timeInterval secsToBeAdded: TimeInterval,
    sinceDate date: Date
)
```

``` source
convenience init(
    timeInterval secsToBeAdded: TimeInterval,
    since date: Date
)
```

## Parameters 

`secsToBeAdded`  

The number of seconds to add to `date`. A negative value means the receiver will be earlier than `date`.

`date`  

The reference date.

## Return Value

An `NSDate` object initialized relative to `date` by `secsToBeAdded` seconds.

## See Also

### Initializing a Date

init()

Returns a date object initialized to the current date and time.

convenience init(timeIntervalSinceNow: TimeInterval)

Returns a date object initialized relative to the current date and time by a given number of seconds.

init(timeIntervalSinceReferenceDate: TimeInterval)

Returns a date object initialized relative to 00:00:00 UTC on 1 January 2001 by a given number of seconds.

convenience init(timeIntervalSince1970: TimeInterval)

Returns a date object initialized relative to 00:00:00 UTC on 1 January 1970 by a given number of seconds.

init?(coder: NSCoder)

Returns a date object initialized from data in the given unarchiver.

