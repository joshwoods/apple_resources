

- RealityKit
- NetworkCompatibilityToken
-  NetworkCompatibilityToken.Compatibility 

Enumeration

# NetworkCompatibilityToken.Compatibility

Indicates whether two devices running RealityKit are compatible and able to connect and sync scenes.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS

``` source
enum Compatibility
```

## Topics

### Compatibility indicators

case compatible

An indication that the compared devices are running compatible versions of RealityKit.

case sessionProtocolVersionMismatch

An indication that two peers running incompatible versions of RealityKit can’t sync.

### Comparisons

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (NetworkCompatibilityToken.Compatibility, NetworkCompatibilityToken.Compatibility) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Multipeer synchronization

Loading remote assets in multiplayer apps

Ensure assets load on all connected peers before using them.

class MultipeerConnectivityService

A service that provides scene synchronization among all peers in a multipeer connectivity session.

class NetworkCompatibilityToken

An opaque token used to check the networking compatibility between two peers in a multipeer connection.

protocol TransientComponent

An interface for components that aren’t saved to file or cloned.

