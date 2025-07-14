

- AVFAudio
-  AVMusicTrackLoopCount 

Enumeration

# AVMusicTrackLoopCount

Options that define the number of times a track loops.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum AVMusicTrackLoopCount
```

## Topics

### Elements

case forever

A track that loops forever.

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

### Handling Music Tracks

class AVMusicTrack

A collection of music events that you can offset, set to a muted state, modify independently from other track events, and send to a specified destination.

func createAndAppendTrack() -> AVMusicTrack

Creates a new music track and appends it to the sequencer’s list.

func reverseEvents()

Reverses the order of all events in all music tracks, including the tempo track.

func removeTrack(AVMusicTrack) -> Bool

Removes the music track from the sequencer.

