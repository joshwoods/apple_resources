

- MapKit
- MKAnnotationView
-  image 

Instance Property

# image

The image the annotation view displays.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

**macOS**

``` source
@MainActor
var image: NSImage? { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var image: UIImage? { get set }
```

## Discussion

Assigning a new image to this property also changes the size of the view’s frame so that it matches the width and height of the new image. The position of the view’s frame doesn’t change.

## See Also

### Getting and setting attributes

var isEnabled: Bool

A Boolean value that indicates whether the annotation is in an enabled state.

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

