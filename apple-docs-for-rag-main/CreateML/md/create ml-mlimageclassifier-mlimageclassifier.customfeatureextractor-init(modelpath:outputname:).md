

- Create ML
- MLImageClassifier
- MLImageClassifier.CustomFeatureExtractor
-  init(modelPath:outputName:) 

Initializer

# init(modelPath:outputName:)

Creates a custom feature extractor given a model file and an optional output layer name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
init(
    modelPath: URL,
    outputName: String? = nil
)
```

## Parameters 

`modelPath`  

The location of the neural network `.mlmodel` which contains the feature extractor.

`outputName`  

The name of a feature extraction layer within the model has one output type of MLMultiArray. Set this value to `nil` if the model, as a whole, accepts an input image and has exactly one output of type MLMultiArray.

