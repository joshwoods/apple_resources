

- Create ML
- MLSoundClassifier
- MLSoundClassifier.DataSource
-  MLSoundClassifier.DataSource.labeledFiles(at:) 

Case

# MLSoundClassifier.DataSource.labeledFiles(at:)

Creates a data source from a folder that contains audio files, each named after the sound they represent.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case labeledFiles(at: URL)
```

## Parameters 

`at`  

URL: The URL to a folder in the file system that contains audio files. The data source uses the first component of each audio file’s name as its classification label.

## Discussion

Create a sound classifier data source from a directory of audio files with the `labeledFiles` case. You must name each file with a sound classification label, followed by a period and an arbitrary string, ending with the file extension. For example, you can name a sound classifier’s training files as `Laughter.3.png`, `Applause.1.jpg`, `Applause.2.jpg`, and so on.

In this example, these audio file names give a sound classifier at least two class labels:

- `Laughter`

- `Applause`

## See Also

### Creating a data source

case labeledDirectories(at: URL)

Creates a data source from a folder with subfolders that each contain audio files.

case filesByLabel([String : [URL]])

Creates a data source from a dictionary.

case features(table: MLDataTable, featureColumn: String, labelColumn: String, parameters: MLSoundClassifier.FeatureExtractionParameters)

Creates a data source from a data table of audio features.

case featuresDataFrame(DataFrame, featureColumn: String, labelColumn: String, parameters: MLSoundClassifier.FeatureExtractionParameters)

Creates a data source from a data frame of audio features.

struct FeatureExtractionParameters

Parameters that affect the process of extracting sound features from audio files.

