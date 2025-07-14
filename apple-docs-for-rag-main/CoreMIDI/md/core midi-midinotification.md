

- Core MIDI
-  MIDINotification 

Structure

# MIDINotification

A message that describes a system state change.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDINotification
```

## Topics

### Inspecting the Notification

enum MIDINotificationMessageID

The types of state changes the system supports.

var messageID: MIDINotificationMessageID

An identifier that describes the type of state change.

var messageSize: UInt32

The size of the message including its ID.

### Initializers

init()

init(messageID: MIDINotificationMessageID, messageSize: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Callbacks

typealias MIDINotifyProc

A callback function for notifying clients of state changes.

