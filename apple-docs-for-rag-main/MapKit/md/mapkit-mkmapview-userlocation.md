

- MapKit
- MKMapView
-  userLocation 

Instance Property

# userLocation

The annotation object that represents the user’s location.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var userLocation: MKUserLocation { get }
```

## See Also

### Displaying the user’s location

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

var showsUserLocation: Bool

A Boolean value that indicates whether the map tries to display the user’s location.

var isUserLocationVisible: Bool

A Boolean value that indicates whether the user’s location is visible in the map view.

var userTrackingMode: MKUserTrackingMode

The mode to use for tracking the user’s location.

func setUserTrackingMode(MKUserTrackingMode, animated: Bool)

Sets the mode to use for tracking the user’s location, with optional animation.

enum MKUserTrackingMode

The mode to use for tracking the user’s location on the map.

