

- AVFAudio
- AVMIDINoteEvent
-  init(channel:key:velocity:duration:) 

Initializer

# init(channel:key:velocity:duration:)

Creates an event with a MIDI channel, key number, velocity, and duration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    channel: UInt32,
    key keyNum: UInt32,
    velocity: UInt32,
    duration: AVMusicTimeStamp
)
```

## Parameters 

`channel`  

The MIDI channel, between `0` and `15`.

`keyNum`  

The MIDI key number, between `0` and `127`.

`velocity`  

The MIDI velocity, between `0` and `127`.

`duration`  

The duration for this note, in beats.

