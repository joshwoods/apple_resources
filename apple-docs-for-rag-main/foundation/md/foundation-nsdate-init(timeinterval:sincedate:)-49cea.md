

- Foundation
- NSDate
-  init(timeInterval:sinceDate:) 

Initializer

# init(timeInterval:sinceDate:)

Creates and returns a date object set to a given number of seconds from the specified date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    timeInterval secsToBeAdded: TimeInterval,
    sinceDate date: Date
)
```

## Parameters 

`secsToBeAdded`  

The number of seconds to add to `date`. Use a negative argument to specify a date and time before `date`.

`date`  

The date.

## Return Value

An `NSDate` object set to `secsToBeAdded` seconds from `date`.

