

- AVFAudio
- AVMIDIMetaEvent
-  AVMIDIMetaEvent.EventType 

Enumeration

# AVMIDIMetaEvent.EventType

Constants that represent the types of meta events.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum EventType
```

## Topics

### Event Types

case copyright

An event type that represents a copyright.

case cuePoint

An event type that represents a cue point.

case endOfTrack

An event type that represents the end of the track.

case instrument

An event type that represents an instrument.

case keySignature

An event type that represents a key signature.

case lyric

An event type that represents a lyric.

case marker

An event type that represents a marker.

case midiChannel

An event type that represents a MIDI channel.

case midiPort

An event type that represents a MIDI port.

case proprietaryEvent

An event type that represents a proprietary event.

case sequenceNumber

An event type that represents a sequence number.

case smpteOffset

An event type that represents a SMPTE time offset.

case tempo

An event type that represents a tempo.

case text

An event type that represents text.

case timeSignature

An event type that represents a time signature.

case trackName

An event type that represents a track name.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Meta Event Type

var type: AVMIDIMetaEvent.EventType

The type of meta event.

