

- PHASE
- PHASESoundEvent
-  PHASESoundEvent.PrepareHandlerReason 

Enumeration

# PHASESoundEvent.PrepareHandlerReason

Indicates the results of sound-event preparation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PrepareHandlerReason
```

## Overview

The sound event prepare(completion:) function passes an instance of this class to its argument completion closure to communicate the results of the call.

## Topics

### Reasons

case prepared

Indicates the completion of sound-event preparation.

case terminated

Indicates sound-event preparation stops abruptly.

case failure

Indicates an error occurs during sound-event preparation.

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

var prepareState: PHASESoundEvent.PrepareState

The status of sound-event preparation.

enum PrepareState

Indicates the state of sound-event preparation.

