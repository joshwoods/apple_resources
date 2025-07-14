

- Create ML
- MLRandomForestClassifier
-  init(checkpoint:) 

Initializer

# init(checkpoint:)

Creates a random forest classifier classifier from a checkpoint.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
init(checkpoint: MLCheckpoint) throws
```

## Parameters 

`checkpoint`  

Training checkpoint.

## Discussion

Throws

`MLCreateError` if the checkpoint can’t be loaded.

## See Also

### Creating and training a random forest classifier

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestClassifier.ModelParameters) throws

Creates a random forest classifier.

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

