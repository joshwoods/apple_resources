

- PHASE
- PHASEEngine
-  pause() 

Instance Method

# pause()

Pauses all audio playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func pause()
```

## Discussion

To resume paused playback, call start().

## See Also

### Controlling and Inspecting Playback State

func start() throws

Starts or resumes all audio playback.

func stop()

Stops all audio playback.

func update()

Processes app commands and increments framework processing.

var renderingState: PHASESoundEvent.RenderingState

The status of the engine’s audio playback.

