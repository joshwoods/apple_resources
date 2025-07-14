

- Create ML
- MLSoundClassifier
- MLSoundClassifier.DataSource
-  MLSoundClassifier.DataSource.filesByLabel(\_:) 

Case

# MLSoundClassifier.DataSource.filesByLabel(\_:)

Creates a data source from a dictionary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
case filesByLabel([String : [URL]])
```

## Parameters 

`dictionary`  

A dictionary that contains a collection of labeled audio files. Each of the dictionary’s keys is a label, and each key’s value is an array of audio-file URLs.

## Discussion

This data source uses each key in the dictionary to label the audio files in its associated URL array. The following code demonstrates how to create a dictionary with two labels, `"Laughter"` and `"Applause"`.

```
// Get the Documents directory URL.
guard let documentsURL = FileManager.default.urls(for: .documentDirectory,
                                                  in: .userDomainMask).first else {
    fatalError("Can't find Documents directory.")
}

// Build a URL to the ~/Documents/Sounds directory, which contains the training data.
let url = documentsURL.appendingPathComponent("Sounds")

// Create a dictionary of arrays of audio file URLs keyed by a label.
let trainingData = [
    "Laughter": [
        url.appendingPathComponent("Laughter.1.aif"),
        url.appendingPathComponent("Laughter.2.wav")
    ],
    "Applause": [
        url.appendingPathComponent("Applause.1.mp3"),
        url.appendingPathComponent("Applause.2.caf")
    ]
]

let soundClassifier = try MLSoundClassifier(trainingData: trainingData)
```

The value for each label key is an array of URLs to audio files of laughter and applause, respectively.

Note

Use a minimum of 10 sound files per label to train a sound classifier.

## See Also

### Creating a data source

case labeledDirectories(at: URL)

Creates a data source from a folder with subfolders that each contain audio files.

case labeledFiles(at: URL)

Creates a data source from a folder that contains audio files, each named after the sound they represent.

case features(table: MLDataTable, featureColumn: String, labelColumn: String, parameters: MLSoundClassifier.FeatureExtractionParameters)

Creates a data source from a data table of audio features.

case featuresDataFrame(DataFrame, featureColumn: String, labelColumn: String, parameters: MLSoundClassifier.FeatureExtractionParameters)

Creates a data source from a data frame of audio features.

struct FeatureExtractionParameters

Parameters that affect the process of extracting sound features from audio files.

