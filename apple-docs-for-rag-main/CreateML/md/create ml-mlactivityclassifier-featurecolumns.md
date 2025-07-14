

- Create ML
- MLActivityClassifier
-  featureColumns 

Instance Property

# featureColumns

The names of the feature columns the activity classifier used during its training session.

macOS 10.15+

``` source
var featureColumns: [String]
```

## Discussion

Changing the value of this property doesn’t retrain the model or affect its behavior.

## See Also

### Inspecting an activity classifier model

var model: MLModel

The underlying Core ML model of the activity classifier stored in memory.

let modelParameters: MLActivityClassifier.ModelParameters

The model configuration parameters the activity classifier used during its training session.

var labelColumn: String

The name of the label column the activity classifier used during its training session.

var recordingFileColumn: String

The name of the column that contains the data files the activity classifier used during its training session.

