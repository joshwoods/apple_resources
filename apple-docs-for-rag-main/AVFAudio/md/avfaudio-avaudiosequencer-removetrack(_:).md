

- AVFAudio
- AVAudioSequencer
-  removeTrack(\_:) 

Instance Method

# removeTrack(\_:)

Removes the music track from the sequencer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func removeTrack(_ track: AVMusicTrack) -> Bool
```

## Parameters 

`track`  

The music track to remove.

## Return Value

A Boolean value that indicates whether the call succeeds.

## Discussion

This method doesn’t destroy the method track since you can reuse it.

## See Also

### Handling Music Tracks

class AVMusicTrack

A collection of music events that you can offset, set to a muted state, modify independently from other track events, and send to a specified destination.

func createAndAppendTrack() -> AVMusicTrack

Creates a new music track and appends it to the sequencer’s list.

func reverseEvents()

Reverses the order of all events in all music tracks, including the tempo track.

enum AVMusicTrackLoopCount

Options that define the number of times a track loops.

