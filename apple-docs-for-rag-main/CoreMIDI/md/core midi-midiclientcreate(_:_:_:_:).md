

- Core MIDI
-  MIDIClientCreate(\_:\_:\_:\_:) 

Function

# MIDIClientCreate(\_:\_:\_:\_:)

Creates a MIDI client.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIClientCreate(
    _ name: CFString,
    _ notifyProc: MIDINotifyProc?,
    _ notifyRefCon: UnsafeMutableRawPointer?,
    _ outClient: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`name`  

The client’s name.

`notifyProc`  

An optional callback function through which the client receives notifications of changes to the system.

`notifyRefCon`  

A void pointer.

`outClient`  

On successful return, points to the newly created MIDI client.

## Return Value

An `OSStatus` result code.

## Discussion

The system invokes the callback function on the same run loop that you created the client on.

## Topics

### Callbacks

typealias MIDINotifyProc

A callback function for notifying clients of state changes.

struct MIDINotification

A message that describes a system state change.

## See Also

### Client management

Incorporating MIDI 2 into your apps

Add precision and improve musical control for your MIDI apps.

func MIDIClientCreateWithBlock(CFString, UnsafeMutablePointer&lt;MIDIClientRef>, MIDINotifyBlock?) -> OSStatus

Creates a MIDI client with a callback block.

func MIDIClientDispose(MIDIClientRef) -> OSStatus

Disposes of a MIDI client.

typealias MIDIClientRef

An object that maintains per-client state.

