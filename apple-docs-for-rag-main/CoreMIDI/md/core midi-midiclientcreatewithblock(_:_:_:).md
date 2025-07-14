

- Core MIDI
-  MIDIClientCreateWithBlock(\_:\_:\_:) 

Function

# MIDIClientCreateWithBlock(\_:\_:\_:)

Creates a MIDI client with a callback block.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func MIDIClientCreateWithBlock(
    _ name: CFString,
    _ outClient: UnsafeMutablePointer,
    _ notifyBlock: MIDINotifyBlock?
) -> OSStatus
```

## Parameters 

`name`  

The client’s name.

`outClient`  

On successful return, points to the newly created MIDI client.

`notifyBlock`  

An optional block on which the client receives notifications of changes to the system. This system calls this block on an arbitrary thread. Thread-safety is the block’s responsibility.

## Return Value

An `OSStatus` result code.

## Topics

### Callbacks

typealias MIDINotifyBlock

A callback block for notifying clients of state changes.

struct MIDINotification

A message that describes a system state change.

## See Also

### Client management

Incorporating MIDI 2 into your apps

Add precision and improve musical control for your MIDI apps.

func MIDIClientCreate(CFString, MIDINotifyProc?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;MIDIClientRef>) -> OSStatus

Creates a MIDI client.

func MIDIClientDispose(MIDIClientRef) -> OSStatus

Disposes of a MIDI client.

typealias MIDIClientRef

An object that maintains per-client state.

