

- Core MIDI
-  MIDIPacketNext(\_:) 

Function

# MIDIPacketNext(\_:)

Advances a MIDI packet pointer to the next packet in a package list.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MIDIPacketNext(_ pkt: UnsafePointer) -> UnsafeMutablePointer
```

## Parameters 

`pkt`  

A pointer to a MIDI packet in a MIDI packet list.

## Return Value

The subsequent packet in the MIDIPacketList.

## See Also

### Packet list management

struct MIDIPacket

A collection of simultaneous MIDI events.

struct MIDIPacketList

A list of MIDI events the system sends to or receives from an endpoint.

typealias MIDITimeStamp

The time on the host clock when the event occurred.

struct UnsafeMutableMIDIPacketListPointer

struct UnsafeMutableMIDIPacketPointer

