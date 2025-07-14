

- MapKit
- MKAnnotationView
-  selectedZPriority 

Instance Property

# selectedZPriority

The relative importance of the annotation view when in a selected state with respect to its ordering along the z-axis.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var selectedZPriority: MKAnnotationViewZPriority { get set }
```

## Discussion

The constant defaultSelected is the default value for selectedZPriority.

## See Also

### Setting the priority for display

var displayPriority: MKFeatureDisplayPriority

The display priority of the annotation view.

struct MKFeatureDisplayPriority

Constants that indicates the display priority for annotations.

var zPriority: MKAnnotationViewZPriority

The relative importance of the annotation view when in an unselected state with respect to its ordering along the z-axis.

struct MKAnnotationViewZPriority

Constants that indicates the priority for ordering overlapping annotation views.

