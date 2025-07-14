

- MapKit
- MKAnnotationView
-  reuseIdentifier 

Instance Property

# reuseIdentifier

The string that identifies that the annotation view is reusable.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var reuseIdentifier: String? { get }
```

## Discussion

You specify the reuse identifier when you create the view. You use this type to retrieve an annotation view that MapKit isn’t currently using because its annotation isn’t onscreen.

If you define distinctly different types of annotations (with distinctly different annotation views to go with them), you can differentiate between the annotation types by specifying different reuse identifiers for each one.

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

var calloutOffset: CGPoint

The offset (in points) at which to place the callout.

