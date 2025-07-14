

- Create ML
- MLActivityClassifier
- MLActivityClassifier.DataSource
-  gatherAnnotatedFeatures(featureColumns:labelColumn:recordingFileColumn:) 

Instance Method

# gatherAnnotatedFeatures(featureColumns:labelColumn:recordingFileColumn:)

Processes the data source and returns a data frame that contains features, labels and file names.

macOS 14.0+

``` source
func gatherAnnotatedFeatures(
    featureColumns: [String],
    labelColumn: String = "label",
    recordingFileColumn: String? = nil
) throws -> DataFrame
```

## Parameters 

`featureColumns`  

The names of the feature columns.

`labelColumn`  

The name of the column with the labels.

`recordingFileColumn`  

The name of the column with the recording file names, if any.

