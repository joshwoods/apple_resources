

- ARKit
- ARGeoAnchor
-  altitude 

Instance Property

# altitude

Vertical distance, in meters, between this anchor and sea level.

iOS 14.0+iPadOS 14.0+

``` source
@nonobjc
var altitude: CLLocationDistance? { get }
```

## Discussion

Negative values indicate below sea level. This property is valid only when altitudeSource is a value other than ARGeoAnchor.AltitudeSource.unknown.

## See Also

### Defining Altitude

var altitudeSource: ARGeoAnchor.AltitudeSource

A record of the source from which an altitude came.

enum AltitudeSource

Options for setting a location anchor’s altitude.

