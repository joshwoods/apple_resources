

- MapKit
- MKMapView
-  isUserLocationVisible 

Instance Property

# isUserLocationVisible

A Boolean value that indicates whether the user’s location is visible in the map view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var isUserLocationVisible: Bool { get }
```

## Discussion

When determining whether the user’s location is visible, this property factors in the horizontal accuracy of the location data. Specifically, if the rectangle that the user’s location represents, plus or minus the horizontal accuracy of that location, intersects the map’s visible rectangle, this property contains the value true. If that location rectangle doesn’t intersect the map’s visible rectangle, this property contains the value false.

When the user’s location is unknown, this property contains the value false.

## See Also

### Displaying the user’s location

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

var showsUserLocation: Bool

A Boolean value that indicates whether the map tries to display the user’s location.

var userLocation: MKUserLocation

The annotation object that represents the user’s location.

var userTrackingMode: MKUserTrackingMode

The mode to use for tracking the user’s location.

func setUserTrackingMode(MKUserTrackingMode, animated: Bool)

Sets the mode to use for tracking the user’s location, with optional animation.

enum MKUserTrackingMode

The mode to use for tracking the user’s location on the map.

