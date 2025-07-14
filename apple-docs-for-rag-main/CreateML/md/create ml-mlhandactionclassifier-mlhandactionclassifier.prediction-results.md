

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.Prediction
-  results 

Instance Property

# results

An array of prediction labels and their confidences for a hand action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var results: [(label: String, confidence: Double)]
```

## See Also

### Inspecting a prediction

var frameRange: Range&lt;Int>

The range of frame rates the hand action classifier used to make its prediction.

