

- MapKit
- MKMapViewDelegate
-  mapView(\_:regionDidChangeAnimated:) 

Instance Method

# mapView(\_:regionDidChangeAnimated:)

Tells the delegate when the region the map view is displaying changes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    regionDidChangeAnimated animated: Bool
)
```

## Parameters 

`mapView`  

The map view with the visible region that changes.

`animated`  

If true, the map view animates the change to the new region.

## Discussion

The map view calls this method at the end of a change to the map’s visible region.

## See Also

### Responding to map position changes

func mapView(MKMapView, regionWillChangeAnimated: Bool)

Tells the delegate when the region the map view is displaying is about to change.

func mapViewDidChangeVisibleRegion(MKMapView)

Tells the delegate when the map view’s visible region changes.

