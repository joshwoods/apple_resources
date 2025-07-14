

- EventKit
- EKAlarm
-  type 

Instance Property

# type

The type of action to trigger when the alarm fires.

macOS 10.8+

``` source
var type: EKAlarmType { get }
```

## Discussion

To set the type of alarm, define one of emailAddress, soundName, or url.

## See Also

### Triggering Alarm Actions

enum EKAlarmType

A value that specifies what type of action occurs when the alarm triggers.

var emailAddress: String?

The recipient of an email to send when the alarm triggers.

var soundName: String?

The name of the sound to play when the alarm triggers.

