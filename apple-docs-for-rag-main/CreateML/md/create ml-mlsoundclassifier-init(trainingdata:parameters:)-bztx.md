

- Create ML
- MLSoundClassifier
-  init(trainingData:parameters:) 

Initializer

# init(trainingData:parameters:)

Creates a sound classifier with a training dataset represented by a data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
init(
    trainingData: MLSoundClassifier.DataSource,
    parameters: MLSoundClassifier.ModelParameters = ModelParameters()
) throws
```

## Parameters 

`trainingData`  

An MLSoundClassifier.DataSource instance that contains a collection of labeled audio files.

`parameters`  

An MLSoundClassifier.ModelParameters instance you use to configure the model for the training session.

## Discussion

Use this initializer to train a sound classifier with an MLSoundClassifier.DataSource. For example, you can organize your audio files into labeled directories. See MLSoundClassifier.DataSource.labeledDirectories(at:).

```
// Get the Documents directory URL.
guard let documentsURL = FileManager.default.urls(for: .documentDirectory,
                                                  in: .userDomainMask).first else {
    fatalError("Can't find Documents directory.")
}

// Build a URL to the ~/Documents/Sounds directory, which contains the training data.
let soundsURL = documentsURL.appendingPathComponent("Sounds")

// The Sounds directory contains subdirectories, one for each class of sound.
// Each subdirectory's name is the label for audio files it contains.
//
// Sounds
// -- Laughter
// -- Recording1.wav
// -- Recording4.wav
// -- ...
// -- Applause
// -- Recording2.wav
// -- Recording5.wav
// -- ...

// Create a data source from the Sounds directory.
let trainingData = MLSoundClassifier.DataSource.labeledDirectories(at: soundsURL)

// Train a sound classifier with the data source.
let soundClassifier = try MLSoundClassifier(trainingData: trainingData)
```

## See Also

### Training a sound classifier synchronously

init(trainingData: [String : [URL]], parameters: MLSoundClassifier.ModelParameters) throws

Creates a sound classifier with a training dataset represented by a dictionary.

Deprecated

