

- Create ML
- MLRandomForestClassifier
-  init(trainingData:targetColumn:featureColumns:parameters:) 

Initializer

# init(trainingData:targetColumn:featureColumns:parameters:)

Creates a random forest classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    trainingData: DataFrame,
    targetColumn: String,
    featureColumns: [String]? = nil,
    parameters: MLRandomForestClassifier.ModelParameters = ModelParameters(validation: .split(strategy: .automatic))
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

### Creating and training a random forest classifier

init(checkpoint: MLCheckpoint) throws

Creates a random forest classifier classifier from a checkpoint.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestClassifier.ModelParameters) throws

Creates a Random Forest Classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLRandomForestClassifier.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

