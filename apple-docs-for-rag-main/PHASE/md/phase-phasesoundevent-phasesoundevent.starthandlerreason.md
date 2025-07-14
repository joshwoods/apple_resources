

- PHASE
- PHASESoundEvent
-  PHASESoundEvent.StartHandlerReason 

Enumeration

# PHASESoundEvent.StartHandlerReason

Indicates the status after starting a sound event.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum StartHandlerReason
```

## Overview

When your app starts a sound event by calling start(completion:), the framework invokes the argument closure when starting succeeds or fails. PHASE passes an instance of this enumeration to the closure to describe the results of the call.

## Topics

### Reasons

case finishedPlaying

Indicates the framework successfully started the sound event.

case terminated

Indicates the framework terminated the sound event abruptly.

case failure

Indicates an error occurred while starting the sound event.

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

### Starting Playback

func start(completion: ((PHASESoundEvent.StartHandlerReason) -> Void)?)

Invokes the sound event and runs the specified code on completion.

