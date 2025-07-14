

- EventKit
- EKAlarm
-  init(relativeOffset:) 

Initializer

# init(relativeOffset:)

Creates and returns an alarm with a relative offset.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
init(relativeOffset offset: TimeInterval)
```

## Parameters 

`offset`  

The offset from the start of an event, at which the alarm fires.

## Return Value

The created alarm.

## Discussion

Negative offset values fire before the start of the event, while positive values fire after the start.

## See Also

### Creating an Alarm

init(absoluteDate: Date)

Creates and returns an alarm with an absolute date.

