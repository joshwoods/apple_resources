

- MapKit
- MKMapViewDelegate
-  mapView(\_:didFailToLocateUserWithError:) 

Instance Method

# mapView(\_:didFailToLocateUserWithError:)

Tells the delegate when an attempt to locate the user’s location fails.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    didFailToLocateUserWithError error: any Error
)
```

## Parameters 

`mapView`  

The map view that’s tracking the user’s location.

`error`  

An error object containing the reason why location tracking fails.

## See Also

### Tracking the user’s location

func mapViewWillStartLocatingUser(MKMapView)

Tells the delegate that the map view is about to start tracking the user’s location.

func mapViewDidStopLocatingUser(MKMapView)

Tells the delegate when the map view stops tracking the user’s location.

func mapView(MKMapView, didUpdate: MKUserLocation)

Tells the delegate when the map view updates the user’s location.

func mapView(MKMapView, didChange: MKUserTrackingMode, animated: Bool)

Tells the delegate when the user-tracking mode changes.

