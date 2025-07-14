

- MapKit
- MKMapViewDelegate
-  mapView(\_:regionWillChangeAnimated:) 

Instance Method

# mapView(\_:regionWillChangeAnimated:)

Tells the delegate when the region the map view is displaying is about to change.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    regionWillChangeAnimated animated: Bool
)
```

## Parameters 

`mapView`  

The map view with the visible region that’s about to change.

`animated`  

If true, the map view animates the change to the new region. If false, the map view makes the change immediately.

## Discussion

The framework calls this method at the beginning of a change to the map’s visible region.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Responding to map position changes

func mapViewDidChangeVisibleRegion(MKMapView)

Tells the delegate when the map view’s visible region changes.

func mapView(MKMapView, regionDidChangeAnimated: Bool)

Tells the delegate when the region the map view is displaying changes.

