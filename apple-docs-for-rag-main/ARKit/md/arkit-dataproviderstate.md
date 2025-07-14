

- ARKit
-  DataProviderState 

Enumeration

# DataProviderState

The possible states of a data provider.

visionOS 1.0+

``` source
enum DataProviderState
```

## Topics

### Getting the state of a data provider

case initialized

The data provider has been created.

case running

The data provider is running.

case stopped

The data provider is stopped.

case paused

The data provider is paused.

### Comparing data provider states

var description: String

A textual representation of the state.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Setup

Setting up access to ARKit data

Check whether your app can use ARKit and respect people’s privacy.

class ARKitSession

The main entry point for receiving data from ARKit.

protocol DataProvider

A source of live data from ARKit.

protocol Anchor

The identity, location, and orientation of an object in world space.

protocol TrackableAnchor

An anchor that can gain and lose its tracking state over the course of a session.

