

- MapKit
- MKMapView
-  userTrackingMode 

Instance Property

# userTrackingMode

The mode to use for tracking the user’s location.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 11.0+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var userTrackingMode: MKUserTrackingMode { get set }
```

## Discussion

Setting the tracking mode to MKUserTrackingMode.follow or MKUserTrackingMode.followWithHeading causes the map view to center the map on that location and begin tracking the user’s location. If it’s zoomed out, the map view automatically zooms in on the user’s location, effectively changing the current visible region.

For possible values, see MKUserTrackingMode.

## See Also

### Displaying the user’s location

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

var showsUserLocation: Bool

A Boolean value that indicates whether the map tries to display the user’s location.

var isUserLocationVisible: Bool

A Boolean value that indicates whether the user’s location is visible in the map view.

var userLocation: MKUserLocation

The annotation object that represents the user’s location.

func setUserTrackingMode(MKUserTrackingMode, animated: Bool)

Sets the mode to use for tracking the user’s location, with optional animation.

enum MKUserTrackingMode

The mode to use for tracking the user’s location on the map.

