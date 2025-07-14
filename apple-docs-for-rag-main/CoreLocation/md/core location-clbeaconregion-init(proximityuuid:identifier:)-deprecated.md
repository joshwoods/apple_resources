

- Core Location
- CLBeaconRegion
-  init(proximityUUID:identifier:) Deprecated

Initializer

# init(proximityUUID:identifier:)

Creates and returns a region object that targets a beacon with the specified UUID.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.15–10.15Deprecated

``` source
init(
    proximityUUID: UUID,
    identifier: String
)
```

Deprecated

Use init(uuid:identifier:) instead.

## Parameters 

`proximityUUID`  

The unique ID of the beacons you’re targeting. This value can’t be `nil`.

`identifier`  

A unique identifier to associate with the returned region object. You use this identifier to differentiate regions within your app. This value can’t be `nil`.

## Return Value

An initialized beacon region object.

## Discussion

This method creates a region that results in the reporting of all beacons with the specified `proximityUUID` value. The system ignores the major and minor values of the beacons.

## See Also

### Deprecated

init(proximityUUID: UUID, major: CLBeaconMajorValue, identifier: String)

Creates and returns a region object that targets a beacon with the specified proximity ID and major value.

Deprecated

init(proximityUUID: UUID, major: CLBeaconMajorValue, minor: CLBeaconMinorValue, identifier: String)

Creates and returns a region object that targets a beacon with the specified proximity ID, major value, and minor value.

Deprecated

var proximityUUID: UUID

The unique ID of the beacons you’re targeting.

Deprecated

