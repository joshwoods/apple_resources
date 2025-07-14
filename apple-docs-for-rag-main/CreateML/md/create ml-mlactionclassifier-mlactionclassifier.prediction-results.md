

- Create ML
- MLActionClassifier
- MLActionClassifier.Prediction
-  results 

Instance Property

# results

An array of prediction labels and their confidences for an action.

macOS 11.0+

``` source
var results: [(label: String, confidence: Double)]
```

## See Also

### Inspecting a prediction

var frameRange: Range&lt;Int>

The range of frame rates the action classifier used to make its prediction.

