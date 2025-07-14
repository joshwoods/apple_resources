

- MapKit
- MKMapView
-  selectedAnnotations 

Instance Property

# selectedAnnotations

The selected annotations.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var selectedAnnotations: [any MKAnnotation] { get set }
```

## Discussion

Assigning a new array to this property selects only the first annotation in the array.

## See Also

### Managing annotation selections

var annotationVisibleRect: CGRect

The visible rectangle where the map is displaying annotation views.

func selectAnnotation(any MKAnnotation, animated: Bool)

Selects the specified annotation and displays a callout view for it.

func deselectAnnotation((any MKAnnotation)?, animated: Bool)

Deselects the specified annotation and hides its callout view.

