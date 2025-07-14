

- AVFAudio
- AVAudioSequencer
-  start() 

Instance Method

# start()

Starts the sequencer’s player.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func start() throws
```

## Discussion

If you don’t call prepareToPlay(), the framework calls it and then starts the player.

## See Also

### Operating an Audio Sequencer

func prepareToPlay()

Gets ready to play the sequence by prerolling all events.

func stop()

Stops the sequencer’s player.

