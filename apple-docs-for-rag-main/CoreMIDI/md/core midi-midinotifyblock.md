

- Core MIDI
-  MIDINotifyBlock 

Type Alias

# MIDINotifyBlock

A callback block for notifying clients of state changes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDINotifyBlock = (UnsafePointer) -> Void
```

## Parameters 

`message`  

A structure that contains information about what changed.

## Discussion

The system calls this block when some aspect of the current MIDI setup changes. The system calls it on an arbitrary thread chosen by the implementation; thread safety is the responsibility of the block.

## See Also

### Callbacks

struct MIDINotification

A message that describes a system state change.

