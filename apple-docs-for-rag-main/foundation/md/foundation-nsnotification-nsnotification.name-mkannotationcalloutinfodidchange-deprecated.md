

- Foundation
- NSNotification
- NSNotification.Name
-  MKAnnotationCalloutInfoDidChange Deprecated

Type Property

# MKAnnotationCalloutInfoDidChange

A property to observe to determine when the title or subtitle information of an annotation object changes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
static let MKAnnotationCalloutInfoDidChange: NSNotification.Name
```

Deprecated

Use KVO notifications instead.

## Discussion

This notification supports legacy applications and is no longer necessary. MapKit tracks changes to the title and subtitle of an annotation using KVO notifications.

