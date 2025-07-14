

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Options
-  showsBuildings Deprecated

Instance Property

# showsBuildings

A Boolean that indicates whether the map displays extruded building information.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.9–15.4DeprecatedtvOS 9.2+visionOS 1.0–2.4Deprecated

``` source
var showsBuildings: Bool { get set }
```

Deprecated

MapKit no longer supports this option.

## Discussion

When you set this property to true and the camera has a pitch angle greater than 0, the map extrudes buildings so that they appear to extend above the map plane, creating a 3D effect. You need to set the mapType property must to MKMapType.standard for the map to display extruded buildings. The default value of this property is true.

## See Also

### Configuring the map data

var preferredConfiguration: MKMapConfiguration

The map configuration style to use for snapshots.

var mapType: MKMapType

The map’s visual style.

Deprecated

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter to use for determining the points of interest that appear in the snapshot.

Deprecated

var showsPointsOfInterest: Bool

A Boolean value that indicates whether the map displays point-of-interest information.

Deprecated

