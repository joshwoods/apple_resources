

- AVFAudio
- AVMIDIPlayer
-  isPlaying 

Instance Property

# isPlaying

A Boolean value that indicates whether the sequence is playing.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var isPlaying: Bool { get }
```

## See Also

### Controlling playback

func prepareToPlay()

Prepares the player to play the sequence by prerolling all events.

func play(AVMIDIPlayerCompletionHandler?)

Plays the MIDI sequence.

func stop()

Stops playing the sequence.

