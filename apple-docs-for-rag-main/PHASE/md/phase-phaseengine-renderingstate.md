

- PHASE
- PHASEEngine
-  renderingState 

Instance Property

# renderingState

The status of the engine’s audio playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var renderingState: PHASESoundEvent.RenderingState { get }
```

## Discussion

Access this property to check the engine’s playback status. The value reflects the state that you control by calling one of the functions: start(), stop(), or pause().

## See Also

### Controlling and Inspecting Playback State

func pause()

Pauses all audio playback.

func start() throws

Starts or resumes all audio playback.

func stop()

Stops all audio playback.

func update()

Processes app commands and increments framework processing.

