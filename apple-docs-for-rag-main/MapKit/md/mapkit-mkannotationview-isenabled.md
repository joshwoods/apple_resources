

- MapKit
- MKAnnotationView
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the annotation is in an enabled state.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

The default value of this property is true. If the value of this property is false, the annotation view ignores touch events and isn’t selectable. Subclasses may also display the annotation contents differently depending on the value of this property.

## See Also

### Getting and setting attributes

var image: UIImage?

The image the annotation view displays.

var isHighlighted: Bool

A Boolean value that indicates whether the map view highlights the annotation view.

var annotation: (any MKAnnotation)?

The annotation object associated with the view.

var centerOffset: CGPoint

The offset (in points) at which to display the view.

var calloutOffset: CGPoint

The offset (in points) at which to place the callout.

var reuseIdentifier: String?

The string that identifies that the annotation view is reusable.

