

- Create ML
- MLSupportVectorClassifier
-  modelParameters Deprecated

Instance Property

# modelParameters

The underlying parameters used when training the model.

macOS 10.14–14.0Deprecated

``` source
let modelParameters: MLSupportVectorClassifier.ModelParameters
```

## See Also

### Creating and training a support vector classifier

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLSupportVectorClassifier.ModelParameters) throws

Creates a support vector classifier.

Deprecated

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLSupportVectorClassifier.ModelParameters) throws

Creates a Support Vector Classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

struct ModelParameters

Parameters that affect the process of training a model.

Deprecated

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

Deprecated

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

Deprecated

