

- Core Location
-  CLBeacon 

Class

# CLBeacon

Information about an observed iBeacon device and its relative distance to a person’s device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.15+

``` source
class CLBeacon
```

## Mentioned in 

Turning an iOS device into an iBeacon device

## Overview

The CLBeacon class represents a beacon that was observed during beacon ranging. You do not create instances of this class directly. The location manager (CLLocationManager) object reports observed beacons to its associated delegate object.

The identity of a beacon is defined by its uuid, major, and minor properties. These values are coded into the beacon itself. For a more thorough description of the meaning of those values, see CLBeaconRegion.

## Topics

### Getting the beacon identity

var uuid: UUID

The UUID that the observed beacon transmitted.

var major: NSNumber

The major value that the observed beacon transmitted.

var minor: NSNumber

The minor value that the observed beacon transmitted.

var proximityUUID: UUID

The proximity ID of the beacon.

Deprecated

### Determining the distance to the beacon

var proximity: CLProximity

The relative distance to the beacon.

enum CLProximity

Constants that reflect the relative distance to a beacon.

var accuracy: CLLocationAccuracy

The accuracy of the proximity value, measured in meters from the beacon.

var rssi: Int

The received signal strength of the beacon, measured in decibels.

### Getting the observation timestamp

var timestamp: Date

A timestamp representing when the beacon was observed.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### iBeacon

Ranging for Beacons

Configure a device to act as a beacon and to detect surrounding beacons.

Determining the proximity to an iBeacon device

Detect beacons and determine the relative distance to them.

Turning an iOS device into an iBeacon device

Broadcast iBeacon signals from an iOS device.

protocol CLCondition

The abstract base class for all other monitor conditions.

