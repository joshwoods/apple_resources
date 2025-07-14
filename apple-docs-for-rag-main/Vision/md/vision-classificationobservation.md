

- Vision
-  ClassificationObservation 

Structure

# ClassificationObservation

An object that represents classification information that an image-analysis request produces.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct ClassificationObservation
```

## Topics

### Creating an observation

init(VNClassificationObservation)

Creates a classification observation.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

var hasPrecisionRecallCurve: Bool

A Boolean value that indicates whether the observation contains precision and recall curves.

let identifier: String

The classification label that identifies the type of observation.

### Determining precision and recall

func hasMinimumPrecision(Float, forRecall: Float) -> Bool

Determines whether the observation has a minimum precision value for a specific recall.

func hasMinimumRecall(Float, forPrecision: Float) -> Bool

Determines whether the observation has a minimum recall value for a specific precision.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- VisionObservation

## See Also

### Machine learning image analysis

struct CoreMLRequest

An image-analysis request that uses a Core ML model to process images.

struct CoreMLFeatureValueObservation

An object that represents a collection of key-value information that a Core ML image-analysis request produces.

struct PixelBufferObservation

An object that represents an image that an image-analysis request produces.

