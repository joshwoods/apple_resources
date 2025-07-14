

- AVFAudio
- AVAudioEngine
-  start() 

Instance Method

# start()

Starts the audio engine.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func start() throws
```

## Discussion

This method calls the prepare() method if you don’t call it after invoking stop(). It then starts the audio hardware through the AVAudioInputNode and AVAudioOutputNode instances in the audio engine. This method throws an error when:

- There’s a problem in the structure of the graph, such as the input can’t route to an output or to a recording tap through converter nodes.

- An AVAudioSession error occurs.

- The driver fails to start the hardware.

## See Also

### Playing Audio

func prepare()

Prepares the audio engine for starting.

var isRunning: Bool

A Boolean value that indicates whether the audio engine is running.

func pause()

Pauses the audio engine.

func stop()

Stops the audio engine and releases any previously prepared resources.

func reset()

Resets all audio nodes in the audio engine.

var musicSequence: MusicSequence?

The music sequence instance that you attach to the audio engine, if any.

