

- MapKit
- MKMapView
-  annotations 

Instance Property

# annotations

The annotations associated with the map view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var annotations: [any MKAnnotation] { get }
```

## Discussion

The objects in this array adopt the MKAnnotation protocol. If the map view has no associated annotations, the value of this property is an empty array.

## See Also

### Annotating the map

func addAnnotation(any MKAnnotation)

Adds the specified annotation to the map view.

func addAnnotations([any MKAnnotation])

Adds an array of annotation objects to the map view.

func removeAnnotation(any MKAnnotation)

Removes the specified annotation object from the map view.

func removeAnnotations([any MKAnnotation])

Removes an array of annotation objects from the map view.

func annotations(in: MKMapRect) -> Set&lt;AnyHashable>

Returns the annotation objects within the specified map rectangle.

