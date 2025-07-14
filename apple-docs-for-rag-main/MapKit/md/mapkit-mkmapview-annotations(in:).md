

- MapKit
- MKMapView
-  annotations(in:) 

Instance Method

# annotations(in:)

Returns the annotation objects within the specified map rectangle.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func annotations(in mapRect: MKMapRect) -> Set
```

## Parameters 

`mapRect`  

The portion of the map that you want to search for annotations.

## Return Value

The set of annotation objects within `mapRect`.

## Discussion

This method offers a fast way to retrieve the annotation objects in a particular portion of the map. It’s much faster than doing a linear search of the objects in the annotations property yourself.

## See Also

### Annotating the map

var annotations: [any MKAnnotation]

The annotations associated with the map view.

func addAnnotation(any MKAnnotation)

Adds the specified annotation to the map view.

func addAnnotations([any MKAnnotation])

Adds an array of annotation objects to the map view.

func removeAnnotation(any MKAnnotation)

Removes the specified annotation object from the map view.

func removeAnnotations([any MKAnnotation])

Removes an array of annotation objects from the map view.

