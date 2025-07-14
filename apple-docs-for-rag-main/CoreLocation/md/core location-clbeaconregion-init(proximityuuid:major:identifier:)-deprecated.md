

- Core Location
- CLBeaconRegion
-  init(proximityUUID:major:identifier:) Deprecated

Initializer

# init(proximityUUID:major:identifier:)

Creates and returns a region object that targets a beacon with the specified proximity ID and major value.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.15–10.15Deprecated

``` source
init(
    proximityUUID: UUID,
    major: CLBeaconMajorValue,
    identifier: String
)
```

Deprecated

Use init(uuid:major:identifier:) instead.

## Parameters 

`proximityUUID`  

The unique ID of the beacons you’re targeting. This value can’t be `nil`.

`major`  

The major value that you use to identify one or more beacons.

`identifier`  

A unique identifier to associate with the returned region object. You use this identifier to differentiate regions within your app. This value can’t be `nil`.

## Return Value

An initialized beacon region object.

## Discussion

This method creates a region that reports all beacons with the specified `proximityUUID` and `major` values. The system ignores the beacon’s minor value.

## See Also

### Deprecated

init(proximityUUID: UUID, identifier: String)

Creates and returns a region object that targets a beacon with the specified UUID.

Deprecated

init(proximityUUID: UUID, major: CLBeaconMajorValue, minor: CLBeaconMinorValue, identifier: String)

Creates and returns a region object that targets a beacon with the specified proximity ID, major value, and minor value.

Deprecated

var proximityUUID: UUID

The unique ID of the beacons you’re targeting.

Deprecated

