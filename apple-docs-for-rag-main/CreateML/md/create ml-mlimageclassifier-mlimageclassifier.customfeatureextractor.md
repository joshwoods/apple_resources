

- Create ML
- MLImageClassifier
-  MLImageClassifier.CustomFeatureExtractor 

Structure

# MLImageClassifier.CustomFeatureExtractor

A custom feature extractor a training session uses to train an image classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
struct CustomFeatureExtractor
```

## Topics

### Creating a custom feature extractor

init(modelPath: URL, outputName: String?)

Creates a custom feature extractor given a model file and an optional output layer name.

### Configuring a custom feature extractor

var modelPath: URL

The location of a neural network `.mlmodel` file that takes an image as an input.

var outputName: String?

The name of the output from a feature extraction layer within the model.

## Relationships

### Conforms To

- Sendable

## See Also

### Selecting a feature extractor type

case scenePrint(revision: Int?)

A feature extractor trained on millions of images.

case custom(MLImageClassifier.CustomFeatureExtractor)

A feature extractor that you provide as a Core ML model file or a layer within that file.

