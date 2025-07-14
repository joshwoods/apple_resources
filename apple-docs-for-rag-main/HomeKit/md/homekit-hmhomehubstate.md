

- HomeKit
-  HMHomeHubState 

Enumeration

# HMHomeHubState

The possible states of the home hub.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum HMHomeHubState
```

## Topics

### Specifying the State

case connected

The home hub is connected.

case disconnected

The home hub is disconnected.

case notAvailable

No home hub is present.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Querying the state of a home hub

var homeHubState: HMHomeHubState

The state of the home hub.

