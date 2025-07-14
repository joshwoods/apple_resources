

- AVRouting
-  AVCustomRoutingEventReason 

Enumeration

# AVCustomRoutingEventReason

Values that indicate the reason for a routing event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
enum AVCustomRoutingEventReason
```

## Topics

### Reasons

case activate

A value that indicates that a user selects a route in the picker.

case deactivate

A value that indicates that a user deselects a route in the picker.

case reactivate

A value that indicates to reactivate a route a user authorized previously.

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

### Inspecting an event

var route: AVCustomDeviceRoute

A route for the event.

class AVCustomDeviceRoute

An object that represents a custom device route.

var reason: AVCustomRoutingEventReason

A reason for an event, such as a user request to activate or deactivate a route.

