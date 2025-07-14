

- MapKit
- MKMarkerAnnotationView
-  markerTintColor 

Instance Property

# markerTintColor

The background color of the marker balloon.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
@NSCopying @MainActor
var markerTintColor: NSColor? { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@NSCopying @MainActor
var markerTintColor: UIColor? { get set }
```

## Discussion

The default value of this property is `nil`, which applies the standard color that’s appropriate for the current map style.

