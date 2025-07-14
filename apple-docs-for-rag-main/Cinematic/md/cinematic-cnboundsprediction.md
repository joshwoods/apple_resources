

- Cinematic
-  CNBoundsPrediction 

Structure

# CNBoundsPrediction

A structure representing the bounds of the predicted subject.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
struct CNBoundsPrediction
```

## Topics

### Instance Properties

var confidence: Float

A number between 0.0 and 1.0 representing the probability that a defined object is within the bounds.

var normalizedBounds: CGRect

The bounds of the detected object in normalized coordinates where (0.0, 0.0) is the upper-left corner, and (1.0, 1.0) is the lower-right.

## Relationships

### Conforms To

- Sendable

## See Also

### Custom Object Tracking

class CNObjectTracker

An object that converts a normalized point or rectangle into a detection track that tracks an object over time.

