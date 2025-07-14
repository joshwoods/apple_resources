

- Sound Analysis
- SNClassifySoundRequest
-  init(mlModel:) 

Initializer

# init(mlModel:)

Creates a request that uses a custom sound classification model.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(mlModel: MLModel) throws
```

## Parameters 

`mlModel`  

A Core ML sound classification model.

## Mentioned in 

Classifying Sounds in an Audio File

## Discussion

The model you provide must accept audio data as input and produce a classification dictionary output that contains the probability of each category. For example, you can generate a sound classifier model by creating an MLSoundClassifier and training it with your own audio files.

## See Also

### Creating a Request

init(classifierIdentifier: SNClassifierIdentifier) throws

Creates a request that uses the framework’s built-in sound classification model.

struct SNClassifierIdentifier

An identifier that represents the versions of the framework’s sound classifier.

