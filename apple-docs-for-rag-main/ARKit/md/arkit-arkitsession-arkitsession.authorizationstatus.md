

- ARKit
- ARKitSession
-  ARKitSession.AuthorizationStatus 

Enumeration

# ARKitSession.AuthorizationStatus

The authorization states for a type of ARKit data.

visionOS 1.0+

``` source
enum AuthorizationStatus
```

## Topics

### Getting authorization states

case notDetermined

The user hasn’t yet granted or denied permission.

case allowed

The user granted your app permission to use the associated kind of ARKit data.

case denied

The user denied your app permission to use the associated kind of ARKit data.

### Instance Properties

var description: String

A textual representation of AuthorizationStatus

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

enum AuthorizationType

The authorization types you can request from ARKit.

func queryAuthorization(for: [ARKitSession.AuthorizationType]) async -> [ARKitSession.AuthorizationType : ARKitSession.AuthorizationStatus]

Checks whether the current session is authorized for particular authorization types without requesting authorization.

