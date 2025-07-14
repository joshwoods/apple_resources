

- AVFAudio
- AVAudioSequencer
-  prepareToPlay() 

Instance Method

# prepareToPlay()

Gets ready to play the sequence by prerolling all events.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func prepareToPlay()
```

## Discussion

The framework invokes this method automatically on play if you don’t call it, but it may delay startup.

## See Also

### Operating an Audio Sequencer

func start() throws

Starts the sequencer’s player.

func stop()

Stops the sequencer’s player.

