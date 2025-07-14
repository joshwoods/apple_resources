

- Swift Charts
-  AnnotationOverflowResolution 

Structure

# AnnotationOverflowResolution

The behavior for resolving an annotation that extends past a boundary of the chart.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct AnnotationOverflowResolution
```

## Topics

### Structures

struct Boundary

Describes a boundary of a chart for overflow resolution.

struct Strategy

Strategies for annotation overflow resolution.

### Initializers

init(x: AnnotationOverflowResolution.Strategy, y: AnnotationOverflowResolution.Strategy)

Creates an AnnotationOverflowResolution with strategies for the X and Y dimensions.

### Type Properties

static let automatic: AnnotationOverflowResolution

Automatically resolves overflow in each dimension.

## See Also

### Annotations

struct AnnotationContext

Information about an item that you add an annotation to.

struct AnnotationPosition

The position of an annotation.

