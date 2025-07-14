

- MapKit
- MKMapView
-  setUserTrackingMode(\_:animated:) 

Instance Method

# setUserTrackingMode(\_:animated:)

Sets the mode to use for tracking the user’s location, with optional animation.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 11.0+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func setUserTrackingMode(
    _ mode: MKUserTrackingMode,
    animated: Bool
)
```

## Parameters 

`mode`  

The mode for tracking the user’s location. MKUserTrackingMode describes the possible values.

`animated`  

If true, the map animates the change from the current mode to the new mode; otherwise, it doesn’t. This parameter affects only tracking-mode changes. Changes to the user’s location or heading use animation.

## Discussion

Setting the tracking mode to MKUserTrackingMode.follow or MKUserTrackingMode.followWithHeading causes the map view to center the map on that location and begin tracking the user’s location. If it’s zoomed out, the map view automatically zooms in on the user’s location, effectively changing the current visible region.

## See Also

### Related Documentation

func mapView(MKMapView, didChange: MKUserTrackingMode, animated: Bool)

Tells the delegate when the user-tracking mode changes.

func mapView(MKMapView, didUpdate: MKUserLocation)

Tells the delegate when the map view updates the user’s location.

var heading: CLHeading?

The heading of the user’s location.

### Displaying the user’s location

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

var showsUserLocation: Bool

A Boolean value that indicates whether the map tries to display the user’s location.

var isUserLocationVisible: Bool

A Boolean value that indicates whether the user’s location is visible in the map view.

var userLocation: MKUserLocation

The annotation object that represents the user’s location.

var userTrackingMode: MKUserTrackingMode

The mode to use for tracking the user’s location.

enum MKUserTrackingMode

The mode to use for tracking the user’s location on the map.

