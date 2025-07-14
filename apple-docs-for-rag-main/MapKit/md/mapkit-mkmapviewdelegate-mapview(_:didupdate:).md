

- MapKit
- MKMapViewDelegate
-  mapView(\_:didUpdate:) 

Instance Method

# mapView(\_:didUpdate:)

Tells the delegate when the map view updates the user’s location.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    didUpdate userLocation: MKUserLocation
)
```

## Parameters 

`mapView`  

The map view that’s tracking the user’s location.

`userLocation`  

The location object representing the user’s latest location. This property may be `nil`.

## Mentioned in 

Converting a user’s location to a descriptive placemark

## Discussion

While the showsUserLocation property is true, the map view calls this method whenever it receives a new location update. It also calls this method if the map view’s user-tracking mode is MKUserTrackingMode.followWithHeading and the heading changes.

The.map view doesn’t call this method if the app is running in the background. If you want to receive location updates while running in the background, use the Core Location framework.

## See Also

### Tracking the user’s location

func mapViewWillStartLocatingUser(MKMapView)

Tells the delegate that the map view is about to start tracking the user’s location.

func mapViewDidStopLocatingUser(MKMapView)

Tells the delegate when the map view stops tracking the user’s location.

func mapView(MKMapView, didFailToLocateUserWithError: any Error)

Tells the delegate when an attempt to locate the user’s location fails.

func mapView(MKMapView, didChange: MKUserTrackingMode, animated: Bool)

Tells the delegate when the user-tracking mode changes.

