

- Create ML Components
-  ObjectDetectionMetrics 

Structure

# ObjectDetectionMetrics

Metrics for object detection model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct ObjectDetectionMetrics where Label : Comparable, Label : Decodable, Label : Encodable, Label : Hashable
```

## Topics

### Creating a metrics object

init()

### Getting the properties Properties

var defaultConfidenceThreshold: Float

The default confidence threshold. It is used as the confidence threshold for any label which does not have an explicit confidence threshold, while calculating averagePrecision and meanAveragePrecision.

var labels: Set&lt;Label>

A set of labels present in the dataset.

### Calculating the precision

func averageOfAveragePrecisionAtVariedThresholds&lt;Scalar>(predictions: [[DetectedObject&lt;Label>]], annotations: [ObjectDetectionAnnotation&lt;Label>], confidenceThresholds: [Label : Float]) -> [Label : Scalar]

Calculates average of average precision for all the labels, computed at varied bounding box overlap thresholds. The overlap thresholds range is from `[0.05, 0.95]` with a stride of `0.05`.

func averageOfMeanAveragePrecisionAtVariedThresholds&lt;Scalar>(predictions: [[DetectedObject&lt;Label>]], annotations: [ObjectDetectionAnnotation&lt;Label>], confidenceThresholds: [Label : Float]) -> Scalar

Calculates the average of mean average precision, computed at varied bounding box overlap thresholds. The overlap thresholds range is from `[0.05, 0.95]` with a stride of `0.05`.

func averagePrecision&lt;Scalar>(predictions: [[DetectedObject&lt;Label>]], annotations: [ObjectDetectionAnnotation&lt;Label>], confidenceThresholds: [Label : Float], overlapThreshold: Double) -> [Label : Scalar]

Calculates average precision for all the labels at the bounding box overlap threshold.

func meanAveragePrecision&lt;Scalar>(predictions: [[DetectedObject&lt;Label>]], annotations: [ObjectDetectionAnnotation&lt;Label>], confidenceThresholds: [Label : Float], overlapThreshold: Double) -> Scalar

Calculates the mean average precision at the bounding box overlap threshold.

### Extracting labels

static func extractLabels(from: [ObjectDetectionAnnotation&lt;Label>]) -> Set&lt;Label>

Extracts all the labels from a list of annotations.

## Relationships

### Conforms To

- Sendable

## See Also

### Object detection components

struct DetectedObject

An item in a detection result.

struct ObjectDetectionAnnotation

An object detection annotation.

