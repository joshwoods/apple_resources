

- Core Location
- CLBeaconRegion
-  init(proximityUUID:major:minor:identifier:) Deprecated

Initializer

# init(proximityUUID:major:minor:identifier:)

Creates and returns a region object that targets a beacon with the specified proximity ID, major value, and minor value.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.15–10.15Deprecated

``` source
init(
    proximityUUID: UUID,
    major: CLBeaconMajorValue,
    minor: CLBeaconMinorValue,
    identifier: String
)
```

Deprecated

Use init(uuid:major:minor:identifier:) instead.

## Parameters 

`proximityUUID`  

The proximity ID of the beacon you’re targeting. This value can’t be `nil`.

`major`  

The major value that you use to identify one or more beacons.

`minor`  

The minor value that you use to identify a specific beacon.

`identifier`  

A unique identifier to associate with the returned region object. You use this identifier to differentiate regions within your app. This value can’t be `nil`.

## Return Value

An initialized beacon region object.

## Discussion

This method creates a region that reports the beacon with the specified `proximityUUID`, `major`, and `minor` values.

## See Also

### Deprecated

init(proximityUUID: UUID, identifier: String)

Creates and returns a region object that targets a beacon with the specified UUID.

Deprecated

init(proximityUUID: UUID, major: CLBeaconMajorValue, identifier: String)

Creates and returns a region object that targets a beacon with the specified proximity ID and major value.

Deprecated

var proximityUUID: UUID

The unique ID of the beacons you’re targeting.

Deprecated

