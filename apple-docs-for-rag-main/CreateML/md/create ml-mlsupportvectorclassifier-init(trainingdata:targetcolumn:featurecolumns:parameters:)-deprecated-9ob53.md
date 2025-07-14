

- Create ML
- MLSupportVectorClassifier
-  init(trainingData:targetColumn:featureColumns:parameters:) Deprecated

Initializer

# init(trainingData:targetColumn:featureColumns:parameters:)

Creates a Support Vector Classifier from the feature columns in the training data to predict the categories in the target column.

macOS 10.14–13.0Deprecated

``` source
init(
    trainingData: MLDataTable,
    targetColumn: String,
    featureColumns: [String]? = nil,
    parameters: MLSupportVectorClassifier.ModelParameters = ModelParameters(validationData: nil)
) throws
```

Deprecated

Use DataFrame instead of MLDataTable when initializing.

## Parameters 

`trainingData`  

A data table of training examples.

`targetColumn`  

The column name for the values in the training data that the classifier should predict.

`featureColumns`  

The column names for the values in the training data that the classifier uses to predict the target value.

`parameters`  

The model parameters.

## See Also

### Creating and training a support vector classifier

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLSupportVectorClassifier.ModelParameters) throws

Creates a support vector classifier.

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

