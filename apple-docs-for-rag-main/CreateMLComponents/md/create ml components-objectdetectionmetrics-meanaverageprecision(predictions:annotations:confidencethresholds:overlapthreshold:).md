

- Create ML Components
- ObjectDetectionMetrics
-  meanAveragePrecision(predictions:annotations:confidenceThresholds:overlapThreshold:) 

Instance Method

# meanAveragePrecision(predictions:annotations:confidenceThresholds:overlapThreshold:)

Calculates the mean average precision at the bounding box overlap threshold.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func meanAveragePrecision(
    predictions: [[DetectedObject]],
    annotations: [ObjectDetectionAnnotation],
    confidenceThresholds: [Label : Float] = [:],
    overlapThreshold: Double = 0.5
) -> Scalar where Scalar : BinaryFloatingPoint
```

## Parameters 

`predictions`  

A list of all the predictions from an object detection model. Each element in the list is a list of predictions from one image.

`annotations`  

A list of all the annotations. Each element is an `ObjectDetectionAnnotation` object from one image.

`confidenceThresholds`  

Confidence thresholds for each label. The values will always be between 0.0 and 1.0. If any label does not have a threshold, the `defaultConfidenceThreshold` is used for that label. The default value is `[:]`.

`overlapThreshold`  

The overlap threshold for the bounding boxes. The value will always be between 0.0 and 1.0. The default value is `0.5`.

## Return Value

The mean average precision at the overlap threshold.

## See Also

### Calculating the precision

func averageOfAveragePrecisionAtVariedThresholds&lt;Scalar>(predictions: [[DetectedObject&lt;Label>]], annotations: [ObjectDetectionAnnotation&lt;Label>], confidenceThresholds: [Label : Float]) -> [Label : Scalar]

Calculates average of average precision for all the labels, computed at varied bounding box overlap thresholds. The overlap thresholds range is from `[0.05, 0.95]` with a stride of `0.05`.

func averageOfMeanAveragePrecisionAtVariedThresholds&lt;Scalar>(predictions: [[DetectedObject&lt;Label>]], annotations: [ObjectDetectionAnnotation&lt;Label>], confidenceThresholds: [Label : Float]) -> Scalar

Calculates the average of mean average precision, computed at varied bounding box overlap thresholds. The overlap thresholds range is from `[0.05, 0.95]` with a stride of `0.05`.

func averagePrecision&lt;Scalar>(predictions: [[DetectedObject&lt;Label>]], annotations: [ObjectDetectionAnnotation&lt;Label>], confidenceThresholds: [Label : Float], overlapThreshold: Double) -> [Label : Scalar]

Calculates average precision for all the labels at the bounding box overlap threshold.

