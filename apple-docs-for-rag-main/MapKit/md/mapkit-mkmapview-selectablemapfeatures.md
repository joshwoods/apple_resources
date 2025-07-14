

- MapKit
- MKMapView
-  selectableMapFeatures 

Instance Property

# selectableMapFeatures

The property that describes which selectable features the map responds to.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var selectableMapFeatures: MKMapFeatureOptions { get set }
```

## See Also

### Selecting annotations and annotations views

func mapView(MKMapView, didSelect: MKAnnotationView)

Tells the delegate when the user selects one or more of its annotation views.

func mapView(MKMapView, didDeselect: MKAnnotationView)

Tells the delegate when the user deselects one or more of its annotation views.

func mapView(MKMapView, didDeselect: any MKAnnotation)

Tells the delegate when the user deselects one or more annotations.

func mapView(MKMapView, didSelect: any MKAnnotation)

Tells the delegate when the user selects one or more annotations.

