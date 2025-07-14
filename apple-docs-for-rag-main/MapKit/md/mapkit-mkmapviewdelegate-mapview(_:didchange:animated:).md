

- MapKit
- MKMapViewDelegate
-  mapView(\_:didChange:animated:) 

Instance Method

# mapView(\_:didChange:animated:)

Tells the delegate when the user-tracking mode changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 11.0+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    didChange mode: MKUserTrackingMode,
    animated: Bool
)
```

## Parameters 

`mapView`  

The map view where the user-tracking mode changes.

`mode`  

The mode to use for tracking the user’s location.

`animated`  

If true, the map animates the change from the current mode to the new mode; otherwise, the map doesn’t animate the change. This parameter affects only tracking-mode changes. The map animates all changes to the user’s location and heading.

## See Also

### Related Documentation

func setUserTrackingMode(MKUserTrackingMode, animated: Bool)

Sets the mode to use for tracking the user’s location, with optional animation.

### Tracking the user’s location

func mapViewWillStartLocatingUser(MKMapView)

Tells the delegate that the map view is about to start tracking the user’s location.

func mapViewDidStopLocatingUser(MKMapView)

Tells the delegate when the map view stops tracking the user’s location.

func mapView(MKMapView, didUpdate: MKUserLocation)

Tells the delegate when the map view updates the user’s location.

func mapView(MKMapView, didFailToLocateUserWithError: any Error)

Tells the delegate when an attempt to locate the user’s location fails.

