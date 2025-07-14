

- MapKit
- MKAnnotationView
-  accessoryOffset 

Instance Property

# accessoryOffset

An offset that changes the accessory’s default anchor point.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
var accessoryOffset: CGPoint { get set }
```

## See Also

### Managing callout views

var canShowCallout: Bool

A Boolean value that indicates whether the annotation view is able to display extra information in a callout.

var leftCalloutAccessoryView: UIView?

The view to display on the left side of the standard callout.

var rightCalloutAccessoryView: UIView?

The view to display on the right side of the standard callout.

var detailCalloutAccessoryView: UIView?

The detail accessory view to use in the standard callout.

var leftCalloutOffset: CGPoint

The offset in points from the middle-left of the annotation view.

var rightCalloutOffset: CGPoint

The offset in points from the middle-right of the annotation view.

