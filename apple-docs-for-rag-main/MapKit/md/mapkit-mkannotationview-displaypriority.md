

- MapKit
- MKAnnotationView
-  displayPriority 

Instance Property

# displayPriority

The display priority of the annotation view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var displayPriority: MKFeatureDisplayPriority { get set }
```

## Discussion

An annotation view with a priority of required is always visible on the map, whereas other priorities may result in a hidden annotation view. Defaults to `required`.

## See Also

### Setting the priority for display

struct MKFeatureDisplayPriority

Constants that indicates the display priority for annotations.

var zPriority: MKAnnotationViewZPriority

The relative importance of the annotation view when in an unselected state with respect to its ordering along the z-axis.

var selectedZPriority: MKAnnotationViewZPriority

The relative importance of the annotation view when in a selected state with respect to its ordering along the z-axis.

struct MKAnnotationViewZPriority

Constants that indicates the priority for ordering overlapping annotation views.

