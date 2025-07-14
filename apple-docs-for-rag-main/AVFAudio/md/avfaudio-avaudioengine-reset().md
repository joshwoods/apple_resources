

- AVFAudio
- AVAudioEngine
-  reset() 

Instance Method

# reset()

Resets all audio nodes in the audio engine.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func reset()
```

## Discussion

This methods resets all audio nodes in the audio engine. For example, use it to silence reverb and delay tails.

## See Also

### Playing Audio

func prepare()

Prepares the audio engine for starting.

func start() throws

Starts the audio engine.

var isRunning: Bool

A Boolean value that indicates whether the audio engine is running.

func pause()

Pauses the audio engine.

func stop()

Stops the audio engine and releases any previously prepared resources.

var musicSequence: MusicSequence?

The music sequence instance that you attach to the audio engine, if any.

