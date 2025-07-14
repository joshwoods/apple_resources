

- ARKit
- ARKitSession
-  ARKitSession.AuthorizationType 

Enumeration

# ARKitSession.AuthorizationType

The authorization types you can request from ARKit.

visionOS 1.0+

``` source
enum AuthorizationType
```

## Topics

### Requesting authorization

case handTracking

The authorization for access to detailed hand-tracking data.

case worldSensing

The authorization for access to plane detection, scene reconstruction, and image tracking.

case cameraAccess

The authorization for camera access.

### Instance Properties

var description: String

A textual representation of AuthorizationType

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Getting authorization

func requestAuthorization(for: [ARKitSession.AuthorizationType]) async -> [ARKitSession.AuthorizationType : ARKitSession.AuthorizationStatus]

Requests authorization from the user to use the specified kinds of ARKit data.

func queryAuthorization(for: [ARKitSession.AuthorizationType]) async -> [ARKitSession.AuthorizationType : ARKitSession.AuthorizationStatus]

Checks whether the current session is authorized for particular authorization types without requesting authorization.

enum AuthorizationStatus

The authorization states for a type of ARKit data.

