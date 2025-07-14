

- MapKit
- MKMapView
-  addAnnotation(\_:) 

Instance Method

# addAnnotation(\_:)

Adds the specified annotation to the map view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func addAnnotation(_ annotation: any MKAnnotation)
```

## Parameters 

`annotation`  

The annotation object to add to the receiver. This object must conform to the MKAnnotation protocol. The map view retains the specified object.

## See Also

### Annotating the map

var annotations: [any MKAnnotation]

The annotations associated with the map view.

func addAnnotations([any MKAnnotation])

Adds an array of annotation objects to the map view.

func removeAnnotation(any MKAnnotation)

Removes the specified annotation object from the map view.

func removeAnnotations([any MKAnnotation])

Removes an array of annotation objects from the map view.

func annotations(in: MKMapRect) -> Set&lt;AnyHashable>

Returns the annotation objects within the specified map rectangle.

