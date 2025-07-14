

- MapKit
- MKMapViewDelegate
-  mapView(\_:clusterAnnotationForMemberAnnotations:) 

Instance Method

# mapView(\_:clusterAnnotationForMemberAnnotations:)

Asks the delegate to provide a cluster annotation object for the specified annotations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    clusterAnnotationForMemberAnnotations memberAnnotations: [any MKAnnotation]
) -> MKClusterAnnotation
```

## Parameters 

`mapView`  

The map view containing the specified annotations.

`memberAnnotations`  

The annotations for the map to cluster together. The returned MKClusterAnnotation object needs to include the specific annotations in this parameter.

## Return Value

The cluster annotation object.

## Discussion

Use this method to customize the cluster annotations that display on your map. Typically, MapKit creates cluster annotation objects automatically when one or more annotations with the same cluster identifier are too close together. However, you can implement this method and return a custom cluster annotation object for the specified set of annotations.

## See Also

### Managing annotation views

func mapView(MKMapView, viewFor: any MKAnnotation) -> MKAnnotationView?

Returns the view associated with the specified annotation object.

func mapView(MKMapView, didAdd: [MKAnnotationView])

Tells the delegate when the map view adds one or more annotation views to the map.

func mapView(MKMapView, annotationView: MKAnnotationView, calloutAccessoryControlTapped: UIControl)

Tells the delegate when the user taps one of the annotation view’s accessory buttons.

