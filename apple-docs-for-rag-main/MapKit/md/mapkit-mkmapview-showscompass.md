

- MapKit
- MKMapView
-  showsCompass 

Instance Property

# showsCompass

A Boolean value that indicates whether the map displays a compass control.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
@MainActor
var showsCompass: Bool { get set }
```

## Discussion

Use this property to show or hide a control that lets users change the heading orientation of the map.

## See Also

### Configuring the map display

func setCamera(MKMapCamera, animated: Bool)

Changes the camera to use for determining the map’s viewing parameters, and optionally animates the change.

var camera: MKMapCamera

The camera to use for determining the appearance of the map.

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

var showsTraffic: Bool

A Boolean value that indicates whether the map displays traffic information.

Deprecated

