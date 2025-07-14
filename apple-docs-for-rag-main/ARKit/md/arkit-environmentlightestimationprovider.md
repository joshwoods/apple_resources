

- ARKit
-  EnvironmentLightEstimationProvider 

Class

# EnvironmentLightEstimationProvider

A source of live data about lighting information in the environment.

visionOS 2.0+

``` source
final class EnvironmentLightEstimationProvider
```

## Overview

Use the anchor this provider returns to reflect lighting from a person’s surroundings on the surfaces of virtual objects.

## Topics

### Creating an environment light estimation provider

convenience init()

Creates an environment light estimation provider.

### Inspecting the environment light estimation provider

var anchorUpdates: AnchorUpdateSequence&lt;EnvironmentProbeAnchor>

An asynchronous sequence of all anchor updates.

var description: String

A textual representation of this environment light estimation provider.

var state: DataProviderState

The state of an environment light estimation provider.

### Type properties

static var isSupported: Bool

A Boolean value that indicates whether a device supports the environment light estimation provider.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The authorization types that an environment light estimation provider requires.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

## See Also

### Lighting estimation

struct EnvironmentProbeAnchor

An environment probe in the world.

