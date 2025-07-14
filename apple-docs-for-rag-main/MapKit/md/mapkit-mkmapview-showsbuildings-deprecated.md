

- MapKit
- MKMapView
-  showsBuildings Deprecated

Instance Property

# showsBuildings

A Boolean value that indicates whether the map displays extruded building information on supported map types.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.9–15.4DeprecatedtvOS 9.2+visionOS 1.0–2.4Deprecated

``` source
@MainActor
var showsBuildings: Bool { get set }
```

Deprecated

Use MKStandardMapConfiguration instead.

## Discussion

Note

In iOS 16 and macOS 13, and later, when overlay content is present, this property has no effect and the map renders buildings and trees as transparent. This enables content to be clearly visible while preserving the context of the surroundings.

When this property is true and the camera has a pitch angle greater than zero, the map extrudes buildings so that they extend above the map plane, creating a 3D effect. The default value of this property is true.

To display extruded buildings, set the mapType property to MKMapType.standard or MKMapType.mutedStandard.

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

var showsPointsOfInterest: Bool

A Boolean value that indicates whether the map displays point-of-interest information.

Deprecated

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter to use for determining the points of interest that appear on the map.

Deprecated

var showsTraffic: Bool

A Boolean value that indicates whether the map displays traffic information.

Deprecated

