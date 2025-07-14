

- EventKit
- EKAlarm
-  soundName 

Instance Property

# soundName

The name of the sound to play when the alarm triggers.

macOS 10.8+

``` source
var soundName: String? { get set }
```

## Mentioned in 

Setting an alarm

## Discussion

The value of this property is the name of a system sound that can be used with the init(named:) class method to create an `NSSound` object. Assigning this property a value will set the emailAddress and url properties to `nil`.

## See Also

### Triggering Alarm Actions

enum EKAlarmType

A value that specifies what type of action occurs when the alarm triggers.

var type: EKAlarmType

The type of action to trigger when the alarm fires.

var emailAddress: String?

The recipient of an email to send when the alarm triggers.

