

- MapKit
-  MKFeatureDisplayPriority 

Structure

# MKFeatureDisplayPriority

Constants that indicates the display priority for annotations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
struct MKFeatureDisplayPriority
```

## Topics

### Priorities

static let required: MKFeatureDisplayPriority

A constant indicating that the item is required.

static let defaultHigh: MKFeatureDisplayPriority

A constant indicating that the item’s display priority is high.

static let defaultLow: MKFeatureDisplayPriority

A constant indicating that the item’s display priority is low.

### Creating Feature Display Priorities

init(Float)

Creates a feature display priority using the specified floating point value.

init(rawValue: Float)

Creates a feature display priority using the specified raw floating point value.

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

var zPriority: MKAnnotationViewZPriority

The relative importance of the annotation view when in an unselected state with respect to its ordering along the z-axis.

var selectedZPriority: MKAnnotationViewZPriority

The relative importance of the annotation view when in a selected state with respect to its ordering along the z-axis.

struct MKAnnotationViewZPriority

Constants that indicates the priority for ordering overlapping annotation views.

