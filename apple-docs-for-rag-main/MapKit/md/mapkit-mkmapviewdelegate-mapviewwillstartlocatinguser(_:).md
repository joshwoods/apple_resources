

- MapKit
- MKMapViewDelegate
-  mapViewWillStartLocatingUser(\_:) 

Instance Method

# mapViewWillStartLocatingUser(\_:)

Tells the delegate that the map view is about to start tracking the user’s location.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapViewWillStartLocatingUser(_ mapView: MKMapView)
```

## Parameters 

`mapView`  

The map view that’s tracking the user’s location.

## Discussion

The map view calls this method when the value of the showsUserLocation property changes to true.

## See Also

### Tracking the user’s location

func mapViewDidStopLocatingUser(MKMapView)

Tells the delegate when the map view stops tracking the user’s location.

func mapView(MKMapView, didUpdate: MKUserLocation)

Tells the delegate when the map view updates the user’s location.

func mapView(MKMapView, didFailToLocateUserWithError: any Error)

Tells the delegate when an attempt to locate the user’s location fails.

func mapView(MKMapView, didChange: MKUserTrackingMode, animated: Bool)

Tells the delegate when the user-tracking mode changes.

