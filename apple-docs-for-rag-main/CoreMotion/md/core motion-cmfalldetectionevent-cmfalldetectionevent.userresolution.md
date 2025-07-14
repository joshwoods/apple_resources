

- Core Motion
- CMFallDetectionEvent
-  CMFallDetectionEvent.UserResolution 

Enumeration

# CMFallDetectionEvent.UserResolution

User resolutions for fall detection events.

watchOS 7.2+

``` source
enum UserResolution
```

## Overview

The resolution of an event reflects the user’s action in response to the fall detection notification. For example, the user might tap a button to respond inside the notification, or press the digital crown to dismiss the notification.

## Topics

### Resolutions

case confirmed

The user confirmed the event.

case dismissed

The user dismissed the fall event alert, but didn’t explicitly confirm or reject the event.

case rejected

The user rejected the fall event.

case unresponsive

The user didn’t respond to the fall event and the system hasn’t detected recovery motions.

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

### Accessing Fall Data

var resolution: CMFallDetectionEvent.UserResolution

The event’s resolution.

