

- MapKit
-  MKMapViewDefaultClusterAnnotationViewReuseIdentifier 

Global Variable

# MKMapViewDefaultClusterAnnotationViewReuseIdentifier

The default reuse identifier for the annotation view representing a cluster of annotations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
let MKMapViewDefaultClusterAnnotationViewReuseIdentifier: String
```

## Discussion

Use this constant to register a default annotation view to use for clusters of annotations. The map view uses this cluster annotation view when your map view’s delegate doesn’t implement the mapView(_:viewFor:) method, or when that method returns `nil`.

## See Also

### Creating annotation views

func register(AnyClass?, forAnnotationViewWithReuseIdentifier: String)

Registers an annotation view class that the map can create automatically.

func dequeueReusableAnnotationView(withIdentifier: String, for: any MKAnnotation) -> MKAnnotationView

Returns a reusable annotation view using the specified identifier with a specified existing annotation view, if possible.

func dequeueReusableAnnotationView(withIdentifier: String) -> MKAnnotationView?

Returns a reusable annotation view using its identifier.

func view(for: any MKAnnotation) -> MKAnnotationView?

Returns the annotation view associated with the specified annotation object, if any.

let MKMapViewDefaultAnnotationViewReuseIdentifier: String

The default reuse identifier for your map’s annotation views.

