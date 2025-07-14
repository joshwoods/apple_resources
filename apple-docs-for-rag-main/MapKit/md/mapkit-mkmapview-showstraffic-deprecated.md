

- MapKit
- MKMapView
-  showsTraffic Deprecated

Instance Property

# showsTraffic

A Boolean value that indicates whether the map displays traffic information.

iOS 9.0–18.4DeprecatediPadOS 9.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.11–15.4DeprecatedtvOS 9.2+visionOS 1.0–2.4Deprecated

``` source
@MainActor
var showsTraffic: Bool { get set }
```

Deprecated

Use MKStandardMapConfiguration or MKHybridMapConfiguration and configure the `showsTraffic` property instead.

## Discussion

The mapType property must be set to MKMapType.standard or MKMapType.hybrid for traffic information to be shown. The default value of this property is false.

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

var showsPointsOfInterest: Bool

A Boolean value that indicates whether the map displays point-of-interest information.

Deprecated

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter to use for determining the points of interest that appear on the map.

Deprecated

