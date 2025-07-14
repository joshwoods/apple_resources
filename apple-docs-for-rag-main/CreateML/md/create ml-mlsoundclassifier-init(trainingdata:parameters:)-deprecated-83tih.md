

- Create ML
- MLSoundClassifier
-  init(trainingData:parameters:) Deprecated

Initializer

# init(trainingData:parameters:)

Creates a sound classifier with a training dataset represented by a dictionary.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.15–11.0DeprecatedvisionOS 1.0+

``` source
init(
    trainingData: [String : [URL]],
    parameters: MLSoundClassifier.ModelParameters = ModelParameters()
) throws
```

Deprecated

Use DataSource.filesByLabel to provide dictionary training data instead.

## Parameters 

`trainingData`  

A dictionary that contains a collection of labeled audio files. Each of the dictionary’s keys is a label, and each key’s value is an array of audio-file URLs.

`parameters`  

An MLSoundClassifier.ModelParameters instance you use to configure the model for the training session.

## See Also

### Training a sound classifier synchronously

init(trainingData: MLSoundClassifier.DataSource, parameters: MLSoundClassifier.ModelParameters) throws

Creates a sound classifier with a training dataset represented by a data source.

