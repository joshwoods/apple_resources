

- MapKit
- MKAnnotationView
-  detailCalloutAccessoryView 

Instance Property

# detailCalloutAccessoryView

The detail accessory view to use in the standard callout.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.2+visionOS 1.0+

**macOS**

``` source
@MainActor
var detailCalloutAccessoryView: NSView? { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var detailCalloutAccessoryView: UIView? { get set }
```

## See Also

### Managing callout views

var accessoryOffset: CGPoint

An offset that changes the accessory’s default anchor point.

var canShowCallout: Bool

A Boolean value that indicates whether the annotation view is able to display extra information in a callout.

var leftCalloutAccessoryView: UIView?

The view to display on the left side of the standard callout.

var rightCalloutAccessoryView: UIView?

The view to display on the right side of the standard callout.

var leftCalloutOffset: CGPoint

The offset in points from the middle-left of the annotation view.

var rightCalloutOffset: CGPoint

The offset in points from the middle-right of the annotation view.

