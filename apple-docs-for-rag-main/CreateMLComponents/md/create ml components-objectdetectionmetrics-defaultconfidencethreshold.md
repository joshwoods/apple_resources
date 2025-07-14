

- Create ML Components
- ObjectDetectionMetrics
-  defaultConfidenceThreshold 

Instance Property

# defaultConfidenceThreshold

The default confidence threshold. It is used as the confidence threshold for any label which does not have an explicit confidence threshold, while calculating averagePrecision and meanAveragePrecision.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var defaultConfidenceThreshold: Float
```

## See Also

### Getting the properties Properties

var labels: Set&lt;Label>

A set of labels present in the dataset.

