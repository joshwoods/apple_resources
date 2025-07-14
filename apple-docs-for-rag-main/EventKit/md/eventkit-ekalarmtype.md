

- EventKit
-  EKAlarmType 

Enumeration

# EKAlarmType

A value that specifies what type of action occurs when the alarm triggers.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKAlarmType
```

## Topics

### Constants

case display

The alarm displays a message.

case audio

The alarm plays a sound.

case procedure

The alarm opens a URL.

case email

The alarm sends an email.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Triggering Alarm Actions

var type: EKAlarmType

The type of action to trigger when the alarm fires.

var emailAddress: String?

The recipient of an email to send when the alarm triggers.

var soundName: String?

The name of the sound to play when the alarm triggers.

