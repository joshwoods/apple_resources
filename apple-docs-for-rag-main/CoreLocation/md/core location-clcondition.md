

- Core Location
-  CLCondition 

Protocol

# CLCondition

The abstract base class for all other monitor conditions.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
protocol CLCondition : Decodable, Encodable, Sendable
```

## Relationships

### Inherits From

- Decodable
- Encodable
- Sendable

### Conforming Types

- CLMonitor.BeaconIdentityCondition
- CLMonitor.CircularGeographicCondition

## See Also

### iBeacon

Ranging for Beacons

Configure a device to act as a beacon and to detect surrounding beacons.

Determining the proximity to an iBeacon device

Detect beacons and determine the relative distance to them.

Turning an iOS device into an iBeacon device

Broadcast iBeacon signals from an iOS device.

class CLBeacon

Information about an observed iBeacon device and its relative distance to a person’s device.

