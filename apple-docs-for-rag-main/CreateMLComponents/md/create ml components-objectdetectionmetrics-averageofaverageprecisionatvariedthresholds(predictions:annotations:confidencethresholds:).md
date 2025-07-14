

- Create ML Components
- ObjectDetectionMetrics
-  averageOfAveragePrecisionAtVariedThresholds(predictions:annotations:confidenceThresholds:) 

Instance Method

# averageOfAveragePrecisionAtVariedThresholds(predictions:annotations:confidenceThresholds:)

Calculates average of average precision for all the labels, computed at varied bounding box overlap thresholds. The overlap thresholds range is from `[0.05, 0.95]` with a stride of `0.05`.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func averageOfAveragePrecisionAtVariedThresholds(
    predictions: [[DetectedObject]],
    annotations: [ObjectDetectionAnnotation],
    confidenceThresholds: [Label : Float] = [:]
) -> [Label : Scalar] where Scalar : BinaryFloatingPoint
```

## Parameters 

`predictions`  

A list of all the predictions from an object detection model. Each element in the list is a list of predictions from one image.

`annotations`  

A list of all the annotations. Each element is an `ObjectDetectionAnnotation` object from one image.

`confidenceThresholds`  

Confidence thresholds for each label. The values will always be between 0.0 and 1.0. If any label does not have a threshold, the `defaultConfidenceThreshold` is used for that label. The default value is `[:]`.

## Return Value

Average of average precision for all the labels, computed at varied bounding box overlap thresholds.

## See Also

### Calculating the precision

func averageOfMeanAveragePrecisionAtVariedThresholds&lt;Scalar>(predictions: [[DetectedObject&lt;Label>]], annotations: [ObjectDetectionAnnotation&lt;Label>], confidenceThresholds: [Label : Float]) -> Scalar

Calculates the average of mean average precision, computed at varied bounding box overlap thresholds. The overlap thresholds range is from `[0.05, 0.95]` with a stride of `0.05`.

func averagePrecision&lt;Scalar>(predictions: [[DetectedObject&lt;Label>]], annotations: [ObjectDetectionAnnotation&lt;Label>], confidenceThresholds: [Label : Float], overlapThreshold: Double) -> [Label : Scalar]

Calculates average precision for all the labels at the bounding box overlap threshold.

func meanAveragePrecision&lt;Scalar>(predictions: [[DetectedObject&lt;Label>]], annotations: [ObjectDetectionAnnotation&lt;Label>], confidenceThresholds: [Label : Float], overlapThreshold: Double) -> Scalar

Calculates the mean average precision at the bounding box overlap threshold.

