

- Core Location
- CLBeaconRegion
-  proximityUUID Deprecated

Instance Property

# proximityUUID

The unique ID of the beacons you’re targeting.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.15–10.15Deprecated

``` source
var proximityUUID: UUID { get }
```

Deprecated

Use uuid instead.

## Discussion

Typically, the UUID is unique to your company and is the same for all of the beacons that you install. Use the major and minor values to differentiate the beacons in your installation.

## See Also

### Deprecated

init(proximityUUID: UUID, identifier: String)

Creates and returns a region object that targets a beacon with the specified UUID.

Deprecated

init(proximityUUID: UUID, major: CLBeaconMajorValue, identifier: String)

Creates and returns a region object that targets a beacon with the specified proximity ID and major value.

Deprecated

init(proximityUUID: UUID, major: CLBeaconMajorValue, minor: CLBeaconMinorValue, identifier: String)

Creates and returns a region object that targets a beacon with the specified proximity ID, major value, and minor value.

Deprecated

