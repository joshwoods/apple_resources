

- MapKit
- MKAnnotationView
-  leftCalloutAccessoryView 

Instance Property

# leftCalloutAccessoryView

The view to display on the left side of the standard callout.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var leftCalloutAccessoryView: UIView? { get set }
```

**macOS**

``` source
@MainActor
var leftCalloutAccessoryView: NSView? { get set }
```

## Discussion

The default value of this property is `nil`. Typically, you use the left callout view to display information about the annotation or to link to custom information that your app provides.

In an iOS app, if the view you specify is also a descendant of the UIControl class, you can use the map view’s delegate to receive notifications when the user taps your control. If it doesn’t descend from UIControl, your view is responsible for handling any touch events within its bounds.

In a macOS app, the callout view’s view controller can implement an action method that responds when the user clicks the control in a callout view.

## See Also

### Managing callout views

var accessoryOffset: CGPoint

An offset that changes the accessory’s default anchor point.

var canShowCallout: Bool

A Boolean value that indicates whether the annotation view is able to display extra information in a callout.

var rightCalloutAccessoryView: UIView?

The view to display on the right side of the standard callout.

var detailCalloutAccessoryView: UIView?

The detail accessory view to use in the standard callout.

var leftCalloutOffset: CGPoint

The offset in points from the middle-left of the annotation view.

var rightCalloutOffset: CGPoint

The offset in points from the middle-right of the annotation view.

