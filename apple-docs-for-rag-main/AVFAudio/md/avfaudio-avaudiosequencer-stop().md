

- AVFAudio
- AVAudioSequencer
-  stop() 

Instance Method

# stop()

Stops the sequencer’s player.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func stop()
```

## Discussion

Stopping the player leaves it in an unprerolled state, but stores the playback position so that a subsequent call to start() resumes where it stops. This action doesn’t stop an audio engine you associate with it.

## See Also

### Operating an Audio Sequencer

func prepareToPlay()

Gets ready to play the sequence by prerolling all events.

func start() throws

Starts the sequencer’s player.

