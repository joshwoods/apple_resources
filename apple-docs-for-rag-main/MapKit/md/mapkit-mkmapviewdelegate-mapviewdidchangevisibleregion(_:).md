

- MapKit
- MKMapViewDelegate
-  mapViewDidChangeVisibleRegion(\_:) 

Instance Method

# mapViewDidChangeVisibleRegion(\_:)

Tells the delegate when the map view’s visible region changes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
optional func mapViewDidChangeVisibleRegion(_ mapView: MKMapView)
```

## Parameters 

`mapView`  

The map view with the visible region that changes.

## Discussion

Use this method to update the map in response to intermediate changes to the region. The map view calls this method each time the value of its visible region changes.

Important

Because the map may call this method many times during the scrolling of the map, your implementation needs to be lightweight. Use this method to record the new region values or to make fast updates to your app’s interface. Don’t start any long-running synchronous tasks in this method.

## See Also

### Responding to map position changes

func mapView(MKMapView, regionWillChangeAnimated: Bool)

Tells the delegate when the region the map view is displaying is about to change.

func mapView(MKMapView, regionDidChangeAnimated: Bool)

Tells the delegate when the region the map view is displaying changes.

