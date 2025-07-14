

- PHASE
- PHASESoundEvent
-  renderingState 

Instance Property

# renderingState

The sound event’s playback status.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var renderingState: PHASESoundEvent.RenderingState { get }
```

## Discussion

Access this property to check the sound event’s playback status. The value reflects the state you control by calling one of the functions: start(completion:), stopAndInvalidate(), or pause().

## See Also

### Checking Playback Status

enum RenderingState

The playback status of audio.

