

- ARKit
-  TrackableAnchor 

Protocol

# TrackableAnchor

An anchor that can gain and lose its tracking state over the course of a session.

visionOS 1.0+

``` source
protocol TrackableAnchor : Anchor
```

## Topics

### Checking an anchor’s tracking state

var isTracked: Bool

A Boolean value that indicates whether ARKit is tracking an anchor.

**Required**

## Relationships

### Inherits From

- Anchor
- CustomStringConvertible
- Identifiable
- Sendable

### Conforming Types

- DeviceAnchor
- HandAnchor
- ImageAnchor
- ObjectAnchor
- WorldAnchor

## See Also

### Setup

Setting up access to ARKit data

Check whether your app can use ARKit and respect people’s privacy.

class ARKitSession

The main entry point for receiving data from ARKit.

protocol DataProvider

A source of live data from ARKit.

enum DataProviderState

The possible states of a data provider.

protocol Anchor

The identity, location, and orientation of an object in world space.

