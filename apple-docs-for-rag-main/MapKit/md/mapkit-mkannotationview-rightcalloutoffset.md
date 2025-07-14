

- MapKit
- MKAnnotationView
-  rightCalloutOffset 

Instance Property

# rightCalloutOffset

The offset in points from the middle-right of the annotation view.

Mac Catalyst 13.0+macOS 10.9+

``` source
@MainActor
var rightCalloutOffset: CGPoint { get set }
```

## Discussion

This property specifies where the map view shows the anchor of the callout when it orients off the right side of the annotation view.

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

var detailCalloutAccessoryView: UIView?

The detail accessory view to use in the standard callout.

var leftCalloutOffset: CGPoint

The offset in points from the middle-left of the annotation view.

