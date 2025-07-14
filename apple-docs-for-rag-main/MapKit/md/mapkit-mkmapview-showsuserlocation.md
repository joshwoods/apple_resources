

- MapKit
- MKMapView
-  showsUserLocation 

Instance Property

# showsUserLocation

A Boolean value that indicates whether the map tries to display the user’s location.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var showsUserLocation: Bool { get set }
```

## Mentioned in 

Converting a user’s location to a descriptive placemark

## Discussion

This property doesn’t indicate whether the user’s location is actually visible on the map, only whether the map view tries to display it. Setting this property to true causes the map view to use the Core Location framework to find the user’s location and try to display it on the map. While this property is true, the map view continues to track the user’s location and update it periodically. The default value of this property is false.

Showing the user’s location doesn’t ensure that it’s visible on the map. The user might scroll the map to a different point, causing the location to be offscreen. To determine whether the user’s location displays on the map, use the isUserLocationVisible property.

## See Also

### Displaying the user’s location

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

var isUserLocationVisible: Bool

A Boolean value that indicates whether the user’s location is visible in the map view.

var userLocation: MKUserLocation

The annotation object that represents the user’s location.

var userTrackingMode: MKUserTrackingMode

The mode to use for tracking the user’s location.

func setUserTrackingMode(MKUserTrackingMode, animated: Bool)

Sets the mode to use for tracking the user’s location, with optional animation.

enum MKUserTrackingMode

The mode to use for tracking the user’s location on the map.

