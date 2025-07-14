

- AVFAudio
- AVAudioEngine
-  stop() 

Instance Method

# stop()

Stops the audio engine and releases any previously prepared resources.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func stop()
```

## Discussion

This method stops the audio engine and the audio hardware, and releases any allocated resources for the prepare() method. When your app doesn’t need to play audio, consider pausing or stopping the engine to minimize power consumption.

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

func reset()

Resets all audio nodes in the audio engine.

var musicSequence: MusicSequence?

The music sequence instance that you attach to the audio engine, if any.

