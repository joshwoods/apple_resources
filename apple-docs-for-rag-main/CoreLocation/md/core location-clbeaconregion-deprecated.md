

- Core Location
-  CLBeaconRegion Deprecated

Class

# CLBeaconRegion

A region for detecting the presence of iBeacon devices.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.15–11.0Deprecated

``` source
class CLBeaconRegion
```

Deprecated

Use CLBeaconIdentityCondition instead.

## Mentioned in 

Turning an iOS device into an iBeacon device

Determining the proximity to an iBeacon device

## Overview

A CLBeaconRegion object defines a region that you use to detect Bluetooth beacons conforming to the iBeacon specification. In contrast to a CLCircularRegion that centers on a geographic location, a CLBeaconRegion focuses on an iBeacon with specific identifying characteristics, which you provide. When a matching device comes in range, Core Location notifies your app.

You monitor beacon regions in two ways. To detect when a beacon is in range, use the startMonitoring(for:) method of your location manager object. After detecting a beacon, call the startRangingBeacons(in:) method to determine the relative distance to that beacon.

When detecting an iBeacon, you need to specify the proximityUUID, major, and minor values that you programmed into the beacon hardware. You use the values to identify your beacons uniquely, and you can specify a subset of values to detect multiple beacons. The proximityUUID property is typically the same for all of the beacons in your installation. Use the major and minor values to distinguish among different beacons in your installation.

If you want to configure the current iOS device as a Bluetooth beacon, create a beacon region with the appropriate identifying information. You can then call the peripheralData(withMeasuredPower:) method of the region to get a dictionary that you can use to advertise the device with the Core Bluetooth framework. For more information about using that framework to advertise the device as a beacon, see Turning an iOS device into an iBeacon device.

For information about how to detect beacons, see Determining the proximity to an iBeacon device.

## Topics

### Creating a beacon region

init(beaconIdentityConstraint: CLBeaconIdentityConstraint, identifier: String)

Creates and returns a region object that targets beacons that satisfy the specified beacon identity constraints.

init(uuid: UUID, identifier: String)

Creates and returns a region object that targets beacons with the specified UUID.

init(uuid: UUID, major: CLBeaconMajorValue, identifier: String)

Creates and returns a region object that targets beacons with the specified UUID and major value.

init(uuid: UUID, major: CLBeaconMajorValue, minor: CLBeaconMinorValue, identifier: String)

Creates and returns a region object that targets beacons with the specified UUID, and major and minor values.

typealias CLBeaconMajorValue

The most significant value in a beacon.

typealias CLBeaconMinorValue

The least significant value in a beacon.

### Getting the beacon identity

var uuid: UUID

The UUID value from the beacon identity constraint that defines the beacon region.

var major: NSNumber?

The major value from the beacon identity constraint that defines the beacon region.

var minor: NSNumber?

The minor value from the beacon identity constraint that defines the beacon region.

var beaconIdentityConstraint: CLBeaconIdentityConstraint

The beacon identity constraint that defines the beacon region.

### Specifying when to send notifications

var notifyEntryStateOnDisplay: Bool

A Boolean value that indicates whether Core Location sends beacon notifications when the device’s display is on.

### Getting the beacon’s advertisement data

func peripheralData(withMeasuredPower: NSNumber?) -> NSMutableDictionary

Retrieves data that you can use to advertise the current device as a beacon.

### Deprecated

init(proximityUUID: UUID, identifier: String)

Creates and returns a region object that targets a beacon with the specified UUID.

init(proximityUUID: UUID, major: CLBeaconMajorValue, identifier: String)

Creates and returns a region object that targets a beacon with the specified proximity ID and major value.

init(proximityUUID: UUID, major: CLBeaconMajorValue, minor: CLBeaconMinorValue, identifier: String)

Creates and returns a region object that targets a beacon with the specified proximity ID, major value, and minor value.

var proximityUUID: UUID

The unique ID of the beacons you’re targeting.

## Relationships

### Inherits From

- CLRegion

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

### Classes

class CLBeaconIdentityConstraint

Identity characteristics that can match one or more beacons.

Deprecated

class CLCircularRegion

A circular geographic region that a center point and radius deine.

Deprecated

