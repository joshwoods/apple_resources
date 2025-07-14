

- AVFAudio
- AVMIDIPitchBendEvent
-  init(channel:value:) 

Initializer

# init(channel:value:)

Creates an event with a channel and pitch bend value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    channel: UInt32,
    value: UInt32
)
```

## Parameters 

`channel`  

The MIDI channel for the message, between `0` and `15`.

`value`  

The pitch bend value, between `0` and `16383`.

