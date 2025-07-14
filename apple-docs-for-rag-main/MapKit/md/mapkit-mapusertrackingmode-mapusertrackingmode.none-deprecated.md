

- MapKit
- MapUserTrackingMode
-  MapUserTrackingMode.none Deprecated

Case

# MapUserTrackingMode.none

The map doesn’t update based on the person’s location.

MapKitSwiftUIiOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac CatalystmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOSwatchOS 7.0–10.0Deprecated

``` source
case none
```

Deprecated

Use Map initializers that take a \`position\` parameter along with\nMapCameraPosition.userLocation to configure the user location\ntracking behavior.

## See Also

### Setting the user tracking mode

case follow

The map updates by following a person’s location.

Deprecated

case followWithHeading

The map updates by following the person’s heading.

