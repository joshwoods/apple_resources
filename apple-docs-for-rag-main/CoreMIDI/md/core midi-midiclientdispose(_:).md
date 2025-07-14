

- Core MIDI
-  MIDIClientDispose(\_:) 

Function

# MIDIClientDispose(\_:)

Disposes of a MIDI client.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIClientDispose(_ client: MIDIClientRef) -> OSStatus
```

## Parameters 

`client`  

The client to dispose of.

## Return Value

An `OSStatus` result code.

## Discussion

Don’t explicitly dispose of your client; the system automatically disposes all clients when an app terminates. However, if you call this method to dispose the last or only client owned by an app, the MIDI server may exit if there are no other clients remaining in the system. If this occurs, all subsequent calls by your app to MIDIClientCreate(_:_:_:_:) and MIDIClientCreateWithBlock(_:_:_:) fail.

## See Also

### Client management

Incorporating MIDI 2 into your apps

Add precision and improve musical control for your MIDI apps.

func MIDIClientCreate(CFString, MIDINotifyProc?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;MIDIClientRef>) -> OSStatus

Creates a MIDI client.

func MIDIClientCreateWithBlock(CFString, UnsafeMutablePointer&lt;MIDIClientRef>, MIDINotifyBlock?) -> OSStatus

Creates a MIDI client with a callback block.

typealias MIDIClientRef

An object that maintains per-client state.

