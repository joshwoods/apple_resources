

- MapKit
- MKMapView
-  removeAnnotation(\_:) 

Instance Method

# removeAnnotation(\_:)

Removes the specified annotation object from the map view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func removeAnnotation(_ annotation: any MKAnnotation)
```

## Parameters 

`annotation`  

The annotation object to remove. This object needs to conform to the MKAnnotation protocol.

## Discussion

If the annotation is associated with an annotation view, and that view has a reuse identifier, this method removes the annotation view and queues it internally for later reuse. You can retrieve queued annotation views (and associate them with new annotations) using the dequeueReusableAnnotationView(withIdentifier:) method.

Removing an annotation object disassociates it from the map view entirely, preventing the map view from displaying it on the map. Typically, you call this method only when you want to hide or delete a specified annotation.

## See Also

### Annotating the map

var annotations: [any MKAnnotation]

The annotations associated with the map view.

func addAnnotation(any MKAnnotation)

Adds the specified annotation to the map view.

func addAnnotations([any MKAnnotation])

Adds an array of annotation objects to the map view.

func removeAnnotations([any MKAnnotation])

Removes an array of annotation objects from the map view.

func annotations(in: MKMapRect) -> Set&lt;AnyHashable>

Returns the annotation objects within the specified map rectangle.

