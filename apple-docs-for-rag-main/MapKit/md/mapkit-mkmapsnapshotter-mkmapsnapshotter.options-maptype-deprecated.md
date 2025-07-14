

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Options
-  mapType Deprecated

Instance Property

# mapType

The map’s visual style.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.9–15.4DeprecatedtvOS 9.2+visionOS 1.0–2.4Deprecated

``` source
var mapType: MKMapType { get set }
```

Deprecated

Use preferredConfiguration instead.

## Discussion

The default value of this property is MKMapType.standard.

## See Also

### Configuring the map data

var preferredConfiguration: MKMapConfiguration

The map configuration style to use for snapshots.

var showsBuildings: Bool

A Boolean that indicates whether the map displays extruded building information.

Deprecated

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter to use for determining the points of interest that appear in the snapshot.

Deprecated

var showsPointsOfInterest: Bool

A Boolean value that indicates whether the map displays point-of-interest information.

Deprecated

