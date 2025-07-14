

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Options
-  showsPointsOfInterest Deprecated

Instance Property

# showsPointsOfInterest

A Boolean value that indicates whether the map displays point-of-interest information.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.2–13.0Deprecated

``` source
var showsPointsOfInterest: Bool { get set }
```

Deprecated

Use pointOfInterestFilter instead.

## Discussion

When this property is set to true, the map displays icons and labels for restaurants, schools, and other relevant points of interest. The default value of this property is true.

## See Also

### Configuring the map data

var preferredConfiguration: MKMapConfiguration

The map configuration style to use for snapshots.

var mapType: MKMapType

The map’s visual style.

Deprecated

var showsBuildings: Bool

A Boolean that indicates whether the map displays extruded building information.

Deprecated

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter to use for determining the points of interest that appear in the snapshot.

Deprecated

