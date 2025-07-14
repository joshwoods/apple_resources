

- Core MIDI
-  MIDITimeStamp 

Type Alias

# MIDITimeStamp

The time on the host clock when the event occurred.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDITimeStamp = UInt64
```

## Discussion

The system determines the timestamp using `mach_absolute_time()`.

## See Also

### Packet list management

func MIDIPacketNext(UnsafePointer&lt;MIDIPacket>) -> UnsafeMutablePointer&lt;MIDIPacket>

Advances a MIDI packet pointer to the next packet in a package list.

struct MIDIPacket

A collection of simultaneous MIDI events.

struct MIDIPacketList

A list of MIDI events the system sends to or receives from an endpoint.

struct UnsafeMutableMIDIPacketListPointer

struct UnsafeMutableMIDIPacketPointer

