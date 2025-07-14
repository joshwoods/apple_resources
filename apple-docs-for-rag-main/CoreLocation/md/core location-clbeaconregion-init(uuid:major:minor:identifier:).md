

- Core Location
- CLBeaconRegion
-  init(uuid:major:minor:identifier:) 

Initializer

# init(uuid:major:minor:identifier:)

Creates and returns a region object that targets beacons with the specified UUID, and major and minor values.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.15–11.0Deprecated

``` source
init(
    uuid: UUID,
    major: CLBeaconMajorValue,
    minor: CLBeaconMinorValue,
    identifier: String
)
```

## Parameters 

`uuid`  

A UUID that identifies the beacons to target.

`major`  

The CLBeaconMajorValue that characterizes beacons for this region to target.

`minor`  

The CLBeaconMinorValue that characterizes beacons for this region to target.

`identifier`  

A unique identifier to associate with the returned region object. You use this identifier to differentiate regions within your app. This value can’t be `nil.`

## See Also

### Creating a beacon region

init(beaconIdentityConstraint: CLBeaconIdentityConstraint, identifier: String)

Creates and returns a region object that targets beacons that satisfy the specified beacon identity constraints.

init(uuid: UUID, identifier: String)

Creates and returns a region object that targets beacons with the specified UUID.

init(uuid: UUID, major: CLBeaconMajorValue, identifier: String)

Creates and returns a region object that targets beacons with the specified UUID and major value.

typealias CLBeaconMajorValue

The most significant value in a beacon.

typealias CLBeaconMinorValue

The least significant value in a beacon.

