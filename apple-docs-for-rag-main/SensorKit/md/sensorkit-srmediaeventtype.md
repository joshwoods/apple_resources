

- SensorKit
-  SRMediaEventType 

Enumeration

# SRMediaEventType

The types of user interaction with media that the sensor tracks.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
enum SRMediaEventType
```

## Topics

### Event types

case onScreen

An event that occurs when the media appears on the screen.

case offScreen

An event that occurs when the media disappears from the screen.

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

### Tracking Media Events

var eventType: SRMediaEventType

The type of user interaction with the media.

