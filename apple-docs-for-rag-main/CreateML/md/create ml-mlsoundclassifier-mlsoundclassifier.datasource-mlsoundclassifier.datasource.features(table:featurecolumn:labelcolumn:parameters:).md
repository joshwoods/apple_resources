

- Create ML
- MLSoundClassifier
- MLSoundClassifier.DataSource
-  MLSoundClassifier.DataSource.features(table:featureColumn:labelColumn:parameters:) 

Case

# MLSoundClassifier.DataSource.features(table:featureColumn:labelColumn:parameters:)

Creates a data source from a data table of audio features.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedvisionOS 1.0+

``` source
case features(
    table: MLDataTable,
    featureColumn: String = __Defaults.featureColumnName,
    labelColumn: String = __Defaults.labelColumnName,
    parameters: MLSoundClassifier.FeatureExtractionParameters = FeatureExtractionParameters()
)
```

## Parameters 

`table`  

An MLDataTable instance that contains labeled audio data.

`featureColumn`  

The name of the column that contains the audio features.

`labelColumn`  

The name of the column that contains the audio labels.

`parameters`  

An MLSoundClassifier.FeatureExtractionParameters instance you use to configure the feature-extraction phase.

## Discussion

Use extractFeatures(trainingData:parameters:sessionParameters:) to create an MLDataTable of audio features.

## See Also

### Creating a data source

case labeledDirectories(at: URL)

Creates a data source from a folder with subfolders that each contain audio files.

case labeledFiles(at: URL)

Creates a data source from a folder that contains audio files, each named after the sound they represent.

case filesByLabel([String : [URL]])

Creates a data source from a dictionary.

case featuresDataFrame(DataFrame, featureColumn: String, labelColumn: String, parameters: MLSoundClassifier.FeatureExtractionParameters)

Creates a data source from a data frame of audio features.

struct FeatureExtractionParameters

Parameters that affect the process of extracting sound features from audio files.

