

- Core MIDI
-  MIDIClientRef 

Type Alias

# MIDIClientRef

An object that maintains per-client state.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDIClientRef = MIDIObjectRef
```

## Discussion

A client object derives from MIDIObjectRef. It doesn’t have an owning object.

## See Also

### Client management

Incorporating MIDI 2 into your apps

Add precision and improve musical control for your MIDI apps.

func MIDIClientCreate(CFString, MIDINotifyProc?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;MIDIClientRef>) -> OSStatus

Creates a MIDI client.

func MIDIClientCreateWithBlock(CFString, UnsafeMutablePointer&lt;MIDIClientRef>, MIDINotifyBlock?) -> OSStatus

Creates a MIDI client with a callback block.

func MIDIClientDispose(MIDIClientRef) -> OSStatus

Disposes of a MIDI client.

