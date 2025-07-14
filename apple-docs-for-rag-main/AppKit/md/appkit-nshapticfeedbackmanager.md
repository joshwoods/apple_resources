

- AppKit
-  NSHapticFeedbackManager 

Class

# NSHapticFeedbackManager

An object that provides access to the haptic feedback management attributes on a system with a Force Touch trackpad.

macOS 10.11+

``` source
class NSHapticFeedbackManager
```

## Topics

### Accessing the Default Feedback Performer

class var defaultPerformer: any NSHapticFeedbackPerformer

Requests a haptic feedback performer object that is based on the current input device, accessibility settings, and user preferences.

### Enumerations

enum FeedbackPattern

A pattern of haptic feedback to be provided to the user.

enum PerformanceTime

A time at which to provide haptic feedback to the user.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Trackpad

class NSPressureConfiguration

An encapsulation of the behavior and progression of a Force Touch trackpad as it responds to specific events.

