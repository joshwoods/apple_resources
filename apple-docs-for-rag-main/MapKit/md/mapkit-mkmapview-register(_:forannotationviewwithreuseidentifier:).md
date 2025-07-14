

- MapKit
- MKMapView
-  register(\_:forAnnotationViewWithReuseIdentifier:) 

Instance Method

# register(\_:forAnnotationViewWithReuseIdentifier:)

Registers an annotation view class that the map can create automatically.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func register(
    _ viewClass: AnyClass?,
    forAnnotationViewWithReuseIdentifier identifier: String
)
```

## Parameters 

`viewClass`  

The class of an annotation view that you use in your map. The class needs to be a subclass of MKAnnotationView.

`identifier`  

The reuse identifier to associate with the specified class. This parameter can’t be `nil` or an empty string.

## Discussion

Use this method to register one or more views that you use to display annotations on your map. Register your classes before adding any annotations to the map.

When you register an annotation view class using this method, the dequeueReusableAnnotationView(withIdentifier:for:) method uses the provided identifier to create the view that you register. It creates a new view only if an existing view isn’t available for reuse.

## See Also

### Creating annotation views

func dequeueReusableAnnotationView(withIdentifier: String, for: any MKAnnotation) -> MKAnnotationView

Returns a reusable annotation view using the specified identifier with a specified existing annotation view, if possible.

func dequeueReusableAnnotationView(withIdentifier: String) -> MKAnnotationView?

Returns a reusable annotation view using its identifier.

func view(for: any MKAnnotation) -> MKAnnotationView?

Returns the annotation view associated with the specified annotation object, if any.

let MKMapViewDefaultAnnotationViewReuseIdentifier: String

The default reuse identifier for your map’s annotation views.

let MKMapViewDefaultClusterAnnotationViewReuseIdentifier: String

The default reuse identifier for the annotation view representing a cluster of annotations.

