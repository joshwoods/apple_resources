

- MapKit
- MKMapView
-  selectAnnotation(\_:animated:) 

Instance Method

# selectAnnotation(\_:animated:)

Selects the specified annotation and displays a callout view for it.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func selectAnnotation(
    _ annotation: any MKAnnotation,
    animated: Bool
)
```

## Parameters 

`annotation`  

The annotation object to select.

`animated`  

If true, the map view animates the callout view into position.

## Discussion

If the specified annotation isn’t onscreen, and, therefore, doesn’t have an associated annotation view, this method has no effect.

## See Also

### Managing annotation selections

var annotationVisibleRect: CGRect

The visible rectangle where the map is displaying annotation views.

var selectedAnnotations: [any MKAnnotation]

The selected annotations.

func deselectAnnotation((any MKAnnotation)?, animated: Bool)

Deselects the specified annotation and hides its callout view.

