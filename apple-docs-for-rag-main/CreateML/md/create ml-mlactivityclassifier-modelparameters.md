

- Create ML
- MLActivityClassifier
-  modelParameters 

Instance Property

# modelParameters

The model configuration parameters the activity classifier used during its training session.

macOS 10.15+

``` source
let modelParameters: MLActivityClassifier.ModelParameters
```

## See Also

### Inspecting an activity classifier model

var model: MLModel

The underlying Core ML model of the activity classifier stored in memory.

var featureColumns: [String]

The names of the feature columns the activity classifier used during its training session.

var labelColumn: String

The name of the label column the activity classifier used during its training session.

var recordingFileColumn: String

The name of the column that contains the data files the activity classifier used during its training session.

