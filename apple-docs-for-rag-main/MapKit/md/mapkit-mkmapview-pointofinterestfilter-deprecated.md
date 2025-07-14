

- MapKit
- MKMapView
-  pointOfInterestFilter Deprecated

Instance Property

# pointOfInterestFilter

The filter to use for determining the points of interest that appear on the map.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0–2.4Deprecated

``` source
@NSCopying @MainActor
var pointOfInterestFilter: MKPointOfInterestFilter? { get set }
```

Deprecated

Use one of the map configurations that support an MKPointOfInterestFilter, such as MKStandardMapConfiguration or MKHybridMapConfiguration instead.

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

var showsTraffic: Bool

A Boolean value that indicates whether the map displays traffic information.

Deprecated

