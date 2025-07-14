

- PHASE
- PHASESoundEvent
-  prepareState 

Instance Property

# prepareState

The status of sound-event preparation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var prepareState: PHASESoundEvent.PrepareState { get }
```

## See Also

### Preparing Playback

func prepare(completion: ((PHASESoundEvent.PrepareHandlerReason) -> Void)?)

Enables a sound event to play and runs the argument code when the sound event plays back.

enum PrepareHandlerReason

Indicates the results of sound-event preparation.

enum PrepareState

Indicates the state of sound-event preparation.

