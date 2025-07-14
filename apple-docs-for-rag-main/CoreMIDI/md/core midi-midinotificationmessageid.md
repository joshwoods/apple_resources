

- Core MIDI
-  MIDINotificationMessageID 

Enumeration

# MIDINotificationMessageID

The types of state changes the system supports.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum MIDINotificationMessageID
```

## Topics

### Change Types

case msgSetupChanged

Some aspect of the current MIDI setup changed.

case msgObjectAdded

The system added a device, entity, or endpoint.

case msgObjectRemoved

The system removed a device, entity, or endpoint.

case msgPropertyChanged

An object’s property value changed.

case msgThruConnectionsChanged

The system created or disposed of a persistent MIDI Thru connection.

case msgSerialPortOwnerChanged

The system changed a serial port owner.

case msgIOError

A driver I/O error occurred.

### Enumeration Cases

case msgInternalStart

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting the Notification

var messageID: MIDINotificationMessageID

An identifier that describes the type of state change.

var messageSize: UInt32

The size of the message including its ID.

