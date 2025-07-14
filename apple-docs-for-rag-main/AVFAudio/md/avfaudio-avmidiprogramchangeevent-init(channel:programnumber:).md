

- AVFAudio
- AVMIDIProgramChangeEvent
-  init(channel:programNumber:) 

Initializer

# init(channel:programNumber:)

Creates a program change event with a channel and program number.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    channel: UInt32,
    programNumber: UInt32
)
```

## Parameters 

`channel`  

The MIDI channel for the message, between `0` and `15`.

`programNumber`  

The program number to send, between `0` and `127`.

## Discussion

The instrument this chooses depends on AVMIDIControlChangeEvent.MessageType.bankSelect events sent prior to this event.

