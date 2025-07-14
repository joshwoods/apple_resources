

- Core Location
-  CLBeaconMajorValue 

Type Alias

# CLBeaconMajorValue

The most significant value in a beacon.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias CLBeaconMajorValue = UInt16
```

## See Also

### Creating a beacon region

init(beaconIdentityConstraint: CLBeaconIdentityConstraint, identifier: String)

Creates and returns a region object that targets beacons that satisfy the specified beacon identity constraints.

init(uuid: UUID, identifier: String)

Creates and returns a region object that targets beacons with the specified UUID.

init(uuid: UUID, major: CLBeaconMajorValue, identifier: String)

Creates and returns a region object that targets beacons with the specified UUID and major value.

init(uuid: UUID, major: CLBeaconMajorValue, minor: CLBeaconMinorValue, identifier: String)

Creates and returns a region object that targets beacons with the specified UUID, and major and minor values.

typealias CLBeaconMinorValue

The least significant value in a beacon.

