

- Create ML
- MLSupportVectorClassifier
-  init(trainingData:targetColumn:featureColumns:parameters:) Deprecated

Initializer

# init(trainingData:targetColumn:featureColumns:parameters:)

Creates a support vector classifier.

macOS 12.0–14.0Deprecated

``` source
init(
    trainingData: DataFrame,
    targetColumn: String,
    featureColumns: [String]? = nil,
    parameters: MLSupportVectorClassifier.ModelParameters = ModelParameters(validation: .split(strategy: .automatic))
) throws
```

## Parameters 

`trainingData`  

The training data

`targetColumn`  

Name of the column containing the class labels

`featureColumns`  

Names of the columns containing feature values. If `nil` all columns, other than the target column, will be used as feature values.

`parameters`  

Model training parameters

## See Also

### Creating and training a support vector classifier

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

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

Deprecated

