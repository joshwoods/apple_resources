

- Swift Charts
- AnnotationOverflowResolution
-  AnnotationOverflowResolution.Strategy 

Structure

# AnnotationOverflowResolution.Strategy

Strategies for annotation overflow resolution.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Strategy
```

## Topics

### Type Properties

static let automatic: AnnotationOverflowResolution.Strategy

Automatically chooses a overflow resolution.

static let disabled: AnnotationOverflowResolution.Strategy

Places the annotation “as-is”.

static let fit: AnnotationOverflowResolution.Strategy

Fits the annotation automatically, adjusting its position to ensure it doesn’t overflow.

static let padScale: AnnotationOverflowResolution.Strategy

Pads the scale of the chart to make space for the annotation.

### Type Methods

static func fit(to: AnnotationOverflowResolution.Boundary) -> AnnotationOverflowResolution.Strategy

Fits the annotation to the given boundary, adjusting its position to ensure it doesn’t overflow.

