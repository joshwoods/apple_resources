

- MapKit
- MKMapView
-  setCamera(\_:animated:) 

Instance Method

# setCamera(\_:animated:)

Changes the camera to use for determining the map’s viewing parameters, and optionally animates the change.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func setCamera(
    _ camera: MKMapCamera,
    animated: Bool
)
```

## Parameters 

`camera`  

The camera object containing the viewing angle information. This parameter can’t be `nil`.

`animated`  

Specify true if you want the map view to animate the change in viewing angle, or false if you want the map to reflect the changes without animations.

## See Also

### Configuring the map display

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

var showsTraffic: Bool

A Boolean value that indicates whether the map displays traffic information.

Deprecated

