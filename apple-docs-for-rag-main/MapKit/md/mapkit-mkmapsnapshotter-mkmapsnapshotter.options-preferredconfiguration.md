

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Options
-  preferredConfiguration 

Instance Property

# preferredConfiguration

The map configuration style to use for snapshots.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@NSCopying
var preferredConfiguration: MKMapConfiguration { get set }
```

## Discussion

Set this property to one of the MKMapConfiguration subclasses to configure the map style to use when making map snapshots.

## See Also

### Configuring the map data

var mapType: MKMapType

The map’s visual style.

Deprecated

var showsBuildings: Bool

A Boolean that indicates whether the map displays extruded building information.

Deprecated

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter to use for determining the points of interest that appear in the snapshot.

Deprecated

var showsPointsOfInterest: Bool

A Boolean value that indicates whether the map displays point-of-interest information.

Deprecated

