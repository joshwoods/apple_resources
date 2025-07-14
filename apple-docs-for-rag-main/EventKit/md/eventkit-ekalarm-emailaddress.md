

- EventKit
- EKAlarm
-  emailAddress 

Instance Property

# emailAddress

The recipient of an email to send when the alarm triggers.

macOS 10.8+

``` source
var emailAddress: String? { get set }
```

## Mentioned in 

Setting an alarm

## Discussion

Assigning this property a value will set the soundName and url properties to `nil`.

## See Also

### Triggering Alarm Actions

enum EKAlarmType

A value that specifies what type of action occurs when the alarm triggers.

var type: EKAlarmType

The type of action to trigger when the alarm fires.

var soundName: String?

The name of the sound to play when the alarm triggers.

