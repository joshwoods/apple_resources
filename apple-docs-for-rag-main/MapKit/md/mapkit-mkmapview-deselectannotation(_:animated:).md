

- MapKit
- MKMapView
-  deselectAnnotation(\_:animated:) 

Instance Method

# deselectAnnotation(\_:animated:)

Deselects the specified annotation and hides its callout view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func deselectAnnotation(
    _ annotation: (any MKAnnotation)?,
    animated: Bool
)
```

## Parameters 

`annotation`  

The annotation object to deselect.

`animated`  

If true, the map view animates the callout view offscreen.

## See Also

### Managing annotation selections

var annotationVisibleRect: CGRect

The visible rectangle where the map is displaying annotation views.

var selectedAnnotations: [any MKAnnotation]

The selected annotations.

func selectAnnotation(any MKAnnotation, animated: Bool)

Selects the specified annotation and displays a callout view for it.

