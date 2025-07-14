

- MapKit
- MKAnnotationView
-  centerOffset 

Instance Property

# centerOffset

The offset (in points) at which to display the view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var centerOffset: CGPoint { get set }
```

## Discussion

By default, the map view places the center point of an annotation view at the coordinate point of the associated annotation. You can use this property to reposition the annotation view as necessary. MapKit measures the x- and y-offset values in points. Positive offset values move the annotation view down and to the right, and negative values move it up and to the left.

## See Also

### Getting and setting attributes

var isEnabled: Bool

A Boolean value that indicates whether the annotation is in an enabled state.

var image: UIImage?

The image the annotation view displays.

var isHighlighted: Bool

A Boolean value that indicates whether the map view highlights the annotation view.

var annotation: (any MKAnnotation)?

The annotation object associated with the view.

var calloutOffset: CGPoint

The offset (in points) at which to place the callout.

var reuseIdentifier: String?

The string that identifies that the annotation view is reusable.

