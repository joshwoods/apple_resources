

- Create ML
- MLSupportVectorClassifier
-  featureColumns Deprecated

Instance Property

# featureColumns

The names of the columns you selected at initialization to train the classifier.

macOS 10.14–14.0Deprecated

``` source
var featureColumns: [String]
```

## Discussion

Changing the value of this property doesn’t retrain the model or affect its behavior.

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

let modelParameters: MLSupportVectorClassifier.ModelParameters

The underlying parameters used when training the model.

Deprecated

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

Deprecated

