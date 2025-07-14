

- ARKit
- ARGeoAnchor
-  ARGeoAnchor.AltitudeSource 

Enumeration

# ARGeoAnchor.AltitudeSource

Options for setting a location anchor’s altitude.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum AltitudeSource
```

## Discussion

Each altitude source has unique performance and accuracy characteristics.

## Topics

### Sources

case precise

The framework sets the altitude using a high-resolution digital-elevation model.

case coarse

The framework sets the altitude using a coarse digital-elevation model.

case userDefined

The app defines the altitude.

case unknown

Altitude isn’t yet set.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Defining Altitude

var altitude: CLLocationDistance?

Vertical distance, in meters, between this anchor and sea level.

var altitudeSource: ARGeoAnchor.AltitudeSource

A record of the source from which an altitude came.

