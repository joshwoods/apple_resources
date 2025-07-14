

- Core Motion
-  CMFallDetectionEvent 

Class

# CMFallDetectionEvent

An object that contains data about a fall detection event.

watchOS 7.2+

``` source
class CMFallDetectionEvent
```

## Topics

### Accessing Fall Data

var resolution: CMFallDetectionEvent.UserResolution

The event’s resolution.

enum UserResolution

User resolutions for fall detection events.

### Getting the event date

var date: Date

The event’s time and date.

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

### Fall detection

class CMFallDetectionManager

An object for managing fall detection events.

protocol CMFallDetectionDelegate

A delegate that receives information about fall detection events and authorization status changes.

NSFallDetectionUsageDescription

A message to the user that explains the app’s request for permission to access fall detection event data.

