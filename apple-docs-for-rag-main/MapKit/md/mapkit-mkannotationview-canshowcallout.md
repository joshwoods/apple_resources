

- MapKit
- MKAnnotationView
-  canShowCallout 

Instance Property

# canShowCallout

A Boolean value that indicates whether the annotation view is able to display extra information in a callout.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var canShowCallout: Bool { get set }
```

## Discussion

If the value of this property is true, the map view shows a standard callout when the user taps a selected annotation view. The callout uses the title and subtitle text from the associated annotation object. If there’s no title text, the map view treats the annotation view as if its isEnabled property is false. The callout also displays any custom callout views in the leftCalloutAccessoryView and rightCalloutAccessoryView properties.

If the value of this property is false, the map view ignores the value of the title and subtitle strings, and the annotation view remains in an enabled state by default. You can still disable the view explicitly using the isEnabled property.

## See Also

### Managing callout views

var accessoryOffset: CGPoint

An offset that changes the accessory’s default anchor point.

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

