

- EventKit
- EKAlarm
-  absoluteDate 

Instance Property

# absoluteDate

The absolute date for the alarm.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var absoluteDate: Date? { get set }
```

## Discussion

If you set this property for a relative offset alarm, it loses the relative offset and becomes an absolute alarm.

## See Also

### Accessing Alarm Dates

var relativeOffset: TimeInterval

The offset from the start of an event, at which the alarm fires.

