

- MapKit
- MKMapViewDelegate
-  mapView(\_:didAdd:) 

Instance Method

# mapView(\_:didAdd:)

Tells the delegate when the map view adds one or more annotation views to the map.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    didAdd views: [MKAnnotationView]
)
```

## Parameters 

`mapView`  

The map view that adds the annotation views.

`views`  

An array of `MKAnnotationView` objects representing the views that the map view adds.

## Discussion

By the time the map view calls this method, MapKit has added the specified views to the map.

## See Also

### Managing annotation views

func mapView(MKMapView, viewFor: any MKAnnotation) -> MKAnnotationView?

Returns the view associated with the specified annotation object.

func mapView(MKMapView, annotationView: MKAnnotationView, calloutAccessoryControlTapped: UIControl)

Tells the delegate when the user taps one of the annotation view’s accessory buttons.

func mapView(MKMapView, clusterAnnotationForMemberAnnotations: [any MKAnnotation]) -> MKClusterAnnotation

Asks the delegate to provide a cluster annotation object for the specified annotations.

