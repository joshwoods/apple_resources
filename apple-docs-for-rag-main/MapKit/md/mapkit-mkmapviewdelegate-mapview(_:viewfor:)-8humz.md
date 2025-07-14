

- MapKit
- MKMapViewDelegate
-  mapView(\_:viewFor:) 

Instance Method

# mapView(\_:viewFor:)

Returns the view associated with the specified annotation object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
optional func mapView(
    _ mapView: MKMapView,
    viewFor annotation: any MKAnnotation
) -> MKAnnotationView?
```

## Parameters 

`mapView`  

The map view that requests the annotation view.

`annotation`  

The object representing the annotation that the map view is about to display. In addition to your custom annotations, this object might be an MKUserLocation object representing the user’s location.

## Return Value

The annotation view to display for the specified annotation, or `nil` if you want to display a standard annotation view.

## Discussion

Rather than create a new view each time the map view calls this method, call the dequeueReusableAnnotationView(withIdentifier:) method of the MKMapView class to see if an existing annotation view of the desired type already exists. If one exists, update the returned view to reflect the attributes of the specified annotation and return it. If a view of the appropriate type doesn’t exist, create one, configure it with the needed annotation data, and return it.

If the object in the `annotation` parameter is an instance of the MKUserLocation class, you can provide a custom view to denote the user’s location. To display the user’s location using the default system view, return `nil`.

If you don’t implement this method, or if you return `nil` from your implementation for annotations other than the user location annotation, the map view uses a standard pin annotation view.

## See Also

### Managing annotation views

func mapView(MKMapView, didAdd: [MKAnnotationView])

Tells the delegate when the map view adds one or more annotation views to the map.

func mapView(MKMapView, annotationView: MKAnnotationView, calloutAccessoryControlTapped: UIControl)

Tells the delegate when the user taps one of the annotation view’s accessory buttons.

func mapView(MKMapView, clusterAnnotationForMemberAnnotations: [any MKAnnotation]) -> MKClusterAnnotation

Asks the delegate to provide a cluster annotation object for the specified annotations.

