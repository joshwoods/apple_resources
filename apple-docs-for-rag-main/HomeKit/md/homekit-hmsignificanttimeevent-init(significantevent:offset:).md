

- HomeKit
- HMSignificantTimeEvent
-  init(significantEvent:offset:) 

Initializer

# init(significantEvent:offset:)

Creates a new significant time event with the specified significant event and offset.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    significantEvent: HMSignificantEvent,
    offset: DateComponents?
)
```

## Parameters 

`significantEvent`  

The significant event for this trigger, for example sunrise.

`offset`  

A date components instance that represents the offset from the significant event that this event fires.

## Return Value

An initialized significant time event which fires at the specified offset from the provided significant event.

## Discussion

To specify that this event should fire before the significant event, supply a date components object with negative values. For example, to specify 30 minutes before sunset, the minute property of the `offset` argument must be set to `-30`.

