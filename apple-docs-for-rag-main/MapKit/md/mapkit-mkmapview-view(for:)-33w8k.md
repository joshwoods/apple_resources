

- MapKit
- MKMapView
-  view(for:) 

Instance Method

# view(for:)

Returns the annotation view associated with the specified annotation object, if any.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func view(for annotation: any MKAnnotation) -> MKAnnotationView?
```

## Parameters 

`annotation`  

The annotation object whose view you want.

## Return Value

The annotation view or `nil` if the view has not yet been created. This method may also return `nil` if the annotation is not in the visible map region and therefore does not have an associated annotation view.

## See Also

### Creating annotation views

func register(AnyClass?, forAnnotationViewWithReuseIdentifier: String)

Registers an annotation view class that the map can create automatically.

func dequeueReusableAnnotationView(withIdentifier: String, for: any MKAnnotation) -> MKAnnotationView

Returns a reusable annotation view using the specified identifier with a specified existing annotation view, if possible.

func dequeueReusableAnnotationView(withIdentifier: String) -> MKAnnotationView?

Returns a reusable annotation view using its identifier.

let MKMapViewDefaultAnnotationViewReuseIdentifier: String

The default reuse identifier for your map’s annotation views.

let MKMapViewDefaultClusterAnnotationViewReuseIdentifier: String

The default reuse identifier for the annotation view representing a cluster of annotations.

