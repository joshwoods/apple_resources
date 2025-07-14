

- PHASE
- PHASESoundEvent
-  PHASESoundEvent.SeekHandlerReason 

Enumeration

# PHASESoundEvent.SeekHandlerReason

Indicates the status after a sound event changes its playback position.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum SeekHandlerReason
```

## Overview

When your app changes the playback position of a sound event by calling seek(to:completion:), the framework invokes the argument closure when the seek succeeds or fails. PHASE passes an instance of this enumeration to the closure to describe the results of the call.

## Topics

### Reasons

case seekSuccessful

Indicates the sound event successfully updated its playback position.

case failureSeekAlreadyInProgress

Indicates the sound event is still updating its playback position.

case failure

Indicates the sound event fails to update its playback position.

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

### Seeking a Time

func seek(to: Double, completion: ((PHASESoundEvent.SeekHandlerReason) -> Void)?)

Advances the sound event’s playback position to a specific time.

