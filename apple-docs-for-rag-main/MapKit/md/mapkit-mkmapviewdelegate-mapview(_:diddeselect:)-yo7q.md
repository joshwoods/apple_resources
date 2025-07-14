

- MapKit
- MKMapViewDelegate
-  mapView(\_:didDeselect:) 

Instance Method

# mapView(\_:didDeselect:)

Tells the delegate when the user deselects one or more of its annotation views.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    didDeselect view: MKAnnotationView
)
```

## Parameters 

`mapView`  

The map view containing the annotation view.

`view`  

The deselected annotation view.

## Discussion

You can use this method to track changes in the selection state of annotation views.

## See Also

### Selecting annotations and annotations views

func mapView(MKMapView, didSelect: MKAnnotationView)

Tells the delegate when the user selects one or more of its annotation views.

func mapView(MKMapView, didDeselect: any MKAnnotation)

Tells the delegate when the user deselects one or more annotations.

func mapView(MKMapView, didSelect: any MKAnnotation)

Tells the delegate when the user selects one or more annotations.

var selectableMapFeatures: MKMapFeatureOptions

The property that describes which selectable features the map responds to.

