

- MapKit
- MKMapView
-  annotationVisibleRect 

Instance Property

# annotationVisibleRect

The visible rectangle where the map is displaying annotation views.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var annotationVisibleRect: CGRect { get }
```

## See Also

### Managing annotation selections

var selectedAnnotations: [any MKAnnotation]

The selected annotations.

func selectAnnotation(any MKAnnotation, animated: Bool)

Selects the specified annotation and displays a callout view for it.

func deselectAnnotation((any MKAnnotation)?, animated: Bool)

Deselects the specified annotation and hides its callout view.

