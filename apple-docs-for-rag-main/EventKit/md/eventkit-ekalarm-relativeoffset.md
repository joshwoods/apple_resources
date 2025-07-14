

- EventKit
- EKAlarm
-  relativeOffset 

Instance Property

# relativeOffset

The offset from the start of an event, at which the alarm fires.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var relativeOffset: TimeInterval { get set }
```

## Discussion

If you set this value for an absolute alarm, it loses its absolute date and becomes a relative offset alarm.

## See Also

### Accessing Alarm Dates

var absoluteDate: Date?

The absolute date for the alarm.

