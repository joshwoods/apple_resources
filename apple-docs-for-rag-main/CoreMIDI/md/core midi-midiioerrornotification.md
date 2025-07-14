

- Core MIDI
-  MIDIIOErrorNotification 

Structure

# MIDIIOErrorNotification

A general I/O error notification.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIIOErrorNotification
```

## Topics

### Creating an error notification

init()

init(messageID: MIDINotificationMessageID, messageSize: UInt32, driverDevice: MIDIDeviceRef, errorCode: OSStatus)

### Inspecting an error notification

var messageID: MIDINotificationMessageID

The type of message.

var messageSize: UInt32

The size of the message.

var driverDevice: MIDIDeviceRef

The device with an I/O error.

var errorCode: OSStatus

The error code of the generated error.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### I/O management

struct MIDISysexSendRequest

A request to asynchronously send a single system-exclusive (SysEx) event to a destination.

struct MIDISysexSendRequestUMP

A request to asynchronously send a single universal MIDI packet (UMP) system-exclusive (SysEx) event to a destination.

func MIDIFlushOutput(MIDIEndpointRef) -> OSStatus

Cancels all pending events that were previously scheduled to send.

func MIDIRestart() -> OSStatus

Stops and restarts MIDI I/O.

