

- AVFAudio
- AVAudioSequencer
-  reverseEvents() 

Instance Method

# reverseEvents()

Reverses the order of all events in all music tracks, including the tempo track.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func reverseEvents()
```

## See Also

### Handling Music Tracks

class AVMusicTrack

A collection of music events that you can offset, set to a muted state, modify independently from other track events, and send to a specified destination.

func createAndAppendTrack() -> AVMusicTrack

Creates a new music track and appends it to the sequencer’s list.

func removeTrack(AVMusicTrack) -> Bool

Removes the music track from the sequencer.

enum AVMusicTrackLoopCount

Options that define the number of times a track loops.

