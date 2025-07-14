

- AVFAudio
- AVMIDIPolyPressureEvent
-  init(channel:key:pressure:) 

Initializer

# init(channel:key:pressure:)

Creates an event with a channel, MIDI key number, and a key pressure value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    channel: UInt32,
    key: UInt32,
    pressure: UInt32
)
```

## Parameters 

`channel`  

The MIDI channel for the message, between `0` and `15`.

`key`  

The MIDI key number to apply the pressure to.

`pressure`  

The poly pressure value.

