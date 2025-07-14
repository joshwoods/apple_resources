

- Create ML
- MLImageClassifier
- MLImageClassifier.CustomFeatureExtractor
-  outputName 

Instance Property

# outputName

The name of the output from a feature extraction layer within the model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
var outputName: String?
```

## Discussion

When training an image classifier with a custom feature extractor, use outputName to select a layer within the model that has an output of MLMultiArray.

Set outputName to `nil` if the model (specified by modelPath) has only one output of type MLMultiArray.

## See Also

### Configuring a custom feature extractor

var modelPath: URL

The location of a neural network `.mlmodel` file that takes an image as an input.

