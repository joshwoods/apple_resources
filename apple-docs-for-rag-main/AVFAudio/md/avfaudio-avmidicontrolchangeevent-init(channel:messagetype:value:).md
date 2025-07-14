

- AVFAudio
- AVMIDIControlChangeEvent
-  init(channel:messageType:value:) 

Initializer

# init(channel:messageType:value:)

Creates an event with a channel, control change type, and a value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    channel: UInt32,
    messageType: AVMIDIControlChangeEvent.MessageType,
    value: UInt32
)
```

## Parameters 

`channel`  

The MIDI channel for the control change, between `0` and `15`.

`messageType`  

The type that indicates which MIDI control change message to send.

`value`  

The value for the control change.

