

- MapKit
-  MKAnnotationViewZPriority 

Structure

# MKAnnotationViewZPriority

Constants that indicates the priority for ordering overlapping annotation views.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct MKAnnotationViewZPriority
```

## Topics

### Priorities

static let defaultSelected: MKAnnotationViewZPriority

The default view overlapping priority for a selected view.

static let defaultUnselected: MKAnnotationViewZPriority

The default view overlapping priority for an unselected view.

static let max: MKAnnotationViewZPriority

The maximum allowed priority for overlapping views.

static let min: MKAnnotationViewZPriority

The minimum allowed priority for overlapping views.

### Initializers

init(Float)

Creates an overlapping priority from the value.

init(rawValue: Float)

Creates an overlapping priority from the value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting the priority for display

var displayPriority: MKFeatureDisplayPriority

The display priority of the annotation view.

struct MKFeatureDisplayPriority

Constants that indicates the display priority for annotations.

var zPriority: MKAnnotationViewZPriority

The relative importance of the annotation view when in an unselected state with respect to its ordering along the z-axis.

var selectedZPriority: MKAnnotationViewZPriority

The relative importance of the annotation view when in a selected state with respect to its ordering along the z-axis.

