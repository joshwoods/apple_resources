

- Create ML
- MLActivityClassifier
-  model 

Instance Property

# model

The underlying Core ML model of the activity classifier stored in memory.

macOS 10.15+

``` source
var model: MLModel { get set }
```

## See Also

### Inspecting an activity classifier model

let modelParameters: MLActivityClassifier.ModelParameters

The model configuration parameters the activity classifier used during its training session.

var featureColumns: [String]

The names of the feature columns the activity classifier used during its training session.

var labelColumn: String

The name of the label column the activity classifier used during its training session.

var recordingFileColumn: String

The name of the column that contains the data files the activity classifier used during its training session.

