

- Core Location
- CLMonitor
-  CLMonitor.BeaconIdentityCondition 

Structure

# CLMonitor.BeaconIdentityCondition

A condition that describes the characteristics of a beacon.

iOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
struct BeaconIdentityCondition
```

## Overview

Use `CLMonitor.BeaconIdentityCondition` to observe events from beacons based on any combination on their UUID, major, or minor characteristics.

## Topics

### Creating a beacon identity condition

init(uuid: UUID)

Creates a beacon identity condition with the UUID characteristic only, and wildcard values for the major and minor characteristics.

init(uuid: UUID, major: UInt16)

Creates a beacon identity condition with UUID and major characteristics, and a wildcard for the minor characteristic.

init(uuid: UUID, major: UInt16, minor: UInt16)

Creates a beacon identity condition with UUID, and major and minor characteristics.

### Instance Properties

let major: UInt16?

let minor: UInt16?

let uuid: UUID

## Relationships

### Conforms To

- CLCondition
- Decodable
- Encodable
- Sendable

## See Also

### Monitor conditions

struct CircularGeographicCondition

A condition that describes a circular geographic area that a center point and radius define.

