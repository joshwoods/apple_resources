

- MapKit
-  MapUserTrackingMode Deprecated

Enumeration

# MapUserTrackingMode

The modes available for user tracking.

MapKitSwiftUIiOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac CatalystmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOSwatchOS 7.0–10.0Deprecated

``` source
enum MapUserTrackingMode
```

Deprecated

Use Map initializers that take a `position` parameter along with `MapCameraPosition.userLocation` to configure how the camera follows the user.

## Topics

### Setting the user tracking mode

case none

The map doesn’t update based on the person’s location.

case follow

The map updates by following a person’s location.

case followWithHeading

The map updates by following the person’s heading.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

