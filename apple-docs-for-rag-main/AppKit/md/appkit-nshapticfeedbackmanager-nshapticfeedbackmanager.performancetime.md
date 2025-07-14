

- AppKit
- NSHapticFeedbackManager
-  NSHapticFeedbackManager.PerformanceTime 

Enumeration

# NSHapticFeedbackManager.PerformanceTime

A time at which to provide haptic feedback to the user.

macOS 10.11+

``` source
enum PerformanceTime
```

## Topics

### Constants

case `default`

Allows the system to choose the most appropriate time for feedback to be provided. Currently, this is the next time the screen is updated.

case now

Instructs the system to provide immediate haptic feedback to the user, rather than waiting for synchronization to occur with something visual occurring on screen.

case drawCompleted

Instructs the system to provide haptic feedback to the user the next time the screen is updated.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum FeedbackPattern

A pattern of haptic feedback to be provided to the user.

