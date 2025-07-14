

- PHASE
- PHASESoundEvent
-  PHASESoundEvent.PrepareState 

Enumeration

# PHASESoundEvent.PrepareState

Indicates the state of sound-event preparation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PrepareState
```

## Topics

### States

case prepareInProgress

Indicates that the sound event prepares for playback.

case prepareNotStarted

Indicates that the sound event awaits preparation.

case prepared

Indicates that the sound event preparation is complete.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Preparing Playback

func prepare(completion: ((PHASESoundEvent.PrepareHandlerReason) -> Void)?)

Enables a sound event to play and runs the argument code when the sound event plays back.

enum PrepareHandlerReason

Indicates the results of sound-event preparation.

var prepareState: PHASESoundEvent.PrepareState

The status of sound-event preparation.

