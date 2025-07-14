

- MapKit
- MKMapView
-  dequeueReusableAnnotationView(withIdentifier:) 

Instance Method

# dequeueReusableAnnotationView(withIdentifier:)

Returns a reusable annotation view using its identifier.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func dequeueReusableAnnotationView(withIdentifier identifier: String) -> MKAnnotationView?
```

## Parameters 

`identifier`  

A string identifying the annotation view for the map view to reuse. This string is the same one you specify when initializing the annotation view using the init(annotation:reuseIdentifier:) method.

## Return Value

An annotation view with the specified identifier, or `nil` if no such object exists in the reuse queue.

## Discussion

For performance reasons, it’s best practice to reuse MKAnnotationView objects in your map views. As annotation views move offscreen, the map view moves them to an internally managed reuse queue. As new annotations move onscreen, and the map view prompts your code to provide a corresponding annotation view, attempt to dequeue an existing view before creating a new one. Dequeueing saves time and memory during performance-critical operations like scrolling.

## See Also

### Creating annotation views

func register(AnyClass?, forAnnotationViewWithReuseIdentifier: String)

Registers an annotation view class that the map can create automatically.

func dequeueReusableAnnotationView(withIdentifier: String, for: any MKAnnotation) -> MKAnnotationView

Returns a reusable annotation view using the specified identifier with a specified existing annotation view, if possible.

func view(for: any MKAnnotation) -> MKAnnotationView?

Returns the annotation view associated with the specified annotation object, if any.

let MKMapViewDefaultAnnotationViewReuseIdentifier: String

The default reuse identifier for your map’s annotation views.

let MKMapViewDefaultClusterAnnotationViewReuseIdentifier: String

The default reuse identifier for the annotation view representing a cluster of annotations.

