

- AVFAudio
- AVMIDIPlayer
-  prepareToPlay() 

Instance Method

# prepareToPlay()

Prepares the player to play the sequence by prerolling all events.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func prepareToPlay()
```

## Discussion

The system automatically calls this method on playback, but calling it in advance minimizes the delay between calling play(_:) and the start of sound output.

## See Also

### Controlling playback

func play(AVMIDIPlayerCompletionHandler?)

Plays the MIDI sequence.

func stop()

Stops playing the sequence.

var isPlaying: Bool

A Boolean value that indicates whether the sequence is playing.

