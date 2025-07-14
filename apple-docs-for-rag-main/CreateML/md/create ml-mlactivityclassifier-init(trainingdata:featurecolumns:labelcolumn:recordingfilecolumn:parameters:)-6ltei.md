

- Create ML
- MLActivityClassifier
-  init(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:) 

Initializer

# init(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:)

Creates an activity classifier with a training dataset represented by a data source.

macOS 10.15+

``` source
init(
    trainingData: MLActivityClassifier.DataSource,
    featureColumns: [String],
    labelColumn: String? = nil,
    recordingFileColumn: String? = nil,
    parameters: MLActivityClassifier.ModelParameters = ModelParameters(validationData: nil)
) throws
```

## Parameters 

`trainingData`  

An MLActivityClassifier.DataSource instance.

`featureColumns`  

The names of the columns in an annotation file that contain sensor data.

`labelColumn`  

The name of the column in an annotation file that contains the activity labels if `trainingData` uses MLActivityClassifier.DataSource.directoryWithDataAndAnnotation(at:annotationFileName:timeStampColumn:labelStartTimeColumn:labelEndTimeColumn:).

The initializer ignores this parameter if `trainingData` uses MLActivityClassifier.DataSource.labeledDirectories(at:).

`recordingFileColumn`  

The name of the column in an annotation file that contains the data filenames if `trainingData` uses MLActivityClassifier.DataSource.directoryWithDataAndAnnotation(at:annotationFileName:timeStampColumn:labelStartTimeColumn:labelEndTimeColumn:).

The initializer ignores this parameter if `trainingData` uses MLActivityClassifier.DataSource.labeledDirectories(at:).

`parameters`  

An MLActivityClassifier.ModelParameters instance you use to configure the model for the training session.

## Discussion

Use this initializer to create an activity classifier with an MLActivityClassifier.DataSource. To configure the training process, initialize the activity classifier with an MLActivityClassifier.ModelParameters instance. For example, you can explicitly define the validation dataset instead of allowing the model to choose a random selection of your training data. Alternatively, set validationData to `nil` to allow the activity classifier to choose the validation data for you from among your training data. This lets you set other parameters — like maximumIterations and batchSize — to nondefault values.

## See Also

### Training an activity classifier synchronously

init(trainingData: MLDataTable, featureColumns: [String], labelColumn: String, recordingFileColumn: String, parameters: MLActivityClassifier.ModelParameters) throws

Creates an activity classifier with a training dataset represented by a data table.

Deprecated

