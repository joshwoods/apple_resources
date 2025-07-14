

- MapKit
- MKMapView
-  showsPointsOfInterest Deprecated

Instance Property

# showsPointsOfInterest

A Boolean value that indicates whether the map displays point-of-interest information.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.2–13.0Deprecated

``` source
@MainActor
var showsPointsOfInterest: Bool { get set }
```

Deprecated

Use pointOfInterestFilter instead.

## Discussion

When this property is set to true, the map displays icons and labels for restaurants, schools, and other relevant points of interest. The mapType property must be set to MKMapType.standard or MKMapType.hybrid for points of interest to be displayed.The default value of this property is true.

## See Also

### Configuring the map display

func setCamera(MKMapCamera, animated: Bool)

Changes the camera to use for determining the map’s viewing parameters, and optionally animates the change.

var camera: MKMapCamera

The camera to use for determining the appearance of the map.

var showsCompass: Bool

A Boolean value that indicates whether the map displays a compass control.

var showsPitchControl: Bool

A Boolean value that indicates whether the map displays the pitch control.

var showsScale: Bool

A Boolean value that indicates whether the map shows scale information.

var showsZoomControls: Bool

A Boolean value that indicates whether the map displays zoom controls.

var showsBuildings: Bool

A Boolean value that indicates whether the map displays extruded building information on supported map types.

Deprecated

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter to use for determining the points of interest that appear on the map.

Deprecated

var showsTraffic: Bool

A Boolean value that indicates whether the map displays traffic information.

Deprecated

