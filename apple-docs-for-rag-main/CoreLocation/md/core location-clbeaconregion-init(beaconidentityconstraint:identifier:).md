

- Core Location
- CLBeaconRegion
-  init(beaconIdentityConstraint:identifier:) 

Initializer

# init(beaconIdentityConstraint:identifier:)

Creates and returns a region object that targets beacons that satisfy the specified beacon identity constraints.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.15–11.0Deprecated

``` source
init(
    beaconIdentityConstraint: CLBeaconIdentityConstraint,
    identifier: String
)
```

## Parameters 

`beaconIdentityConstraint`  

A CLBeaconIdentityConstraint that describes the characteristics of beacons for the framework to target.

`identifier`  

A unique identifier to associate with the returned region object. You use this identifier to differentiate regions within your app. This value can’t be `nil`.

## See Also

### Creating a beacon region

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

