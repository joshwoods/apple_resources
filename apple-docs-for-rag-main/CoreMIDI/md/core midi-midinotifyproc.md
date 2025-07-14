

- Core MIDI
-  MIDINotifyProc 

Type Alias

# MIDINotifyProc

A callback function for notifying clients of state changes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDINotifyProc = (UnsafePointer, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`message`  

A structure that contains information about what changed.

`refCon`  

The client’s `refCon`, passed to MIDIClientCreate(_:_:_:_:).

## Discussion

The system invokes this callback when some aspect of the current MIDI setup changes. The system calls it on the same thread that you called MIDIClientCreate(_:_:_:_:) on.

## See Also

### Callbacks

struct MIDINotification

A message that describes a system state change.

