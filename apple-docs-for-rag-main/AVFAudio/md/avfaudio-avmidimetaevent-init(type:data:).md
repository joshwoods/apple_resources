

- AVFAudio
- AVMIDIMetaEvent
-  init(type:data:) 

Initializer

# init(type:data:)

Creates an event with a MIDI meta event type and data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    type: AVMIDIMetaEvent.EventType,
    data: Data
)
```

## Parameters 

`type`  

The meta event type.

`data`  

The data that contains the contents of the meta event.

