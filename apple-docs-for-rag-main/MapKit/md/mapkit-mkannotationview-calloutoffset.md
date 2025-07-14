

- MapKit
- MKAnnotationView
-  calloutOffset 

Instance Property

# calloutOffset

The offset (in points) at which to place the callout.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var calloutOffset: CGPoint { get set }
```

## Discussion

This property determines the additional distance by which to move the callout. When this property is `(0, 0)`, the map view places the anchor point of the callout on the top-center point of the annotation view’s frame. Specifying positive offset values moves the callout down and to the right, and specifying negative values moves it up and to the left.

MapKit doesn’t use the calloutOffset property in macOS apps. Instead, macOS apps use leftCalloutOffset and rightCalloutOffset.

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

var centerOffset: CGPoint

The offset (in points) at which to display the view.

var reuseIdentifier: String?

The string that identifies that the annotation view is reusable.

