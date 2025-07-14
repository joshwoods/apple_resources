

- AVFAudio
- AVAudioEngine
-  isRunning 

Instance Property

# isRunning

A Boolean value that indicates whether the audio engine is running.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isRunning: Bool { get }
```

## Discussion

The value is true if the audio engine is in a running state; otherwise, false.

## See Also

### Playing Audio

func prepare()

Prepares the audio engine for starting.

func start() throws

Starts the audio engine.

func pause()

Pauses the audio engine.

func stop()

Stops the audio engine and releases any previously prepared resources.

func reset()

Resets all audio nodes in the audio engine.

var musicSequence: MusicSequence?

The music sequence instance that you attach to the audio engine, if any.

