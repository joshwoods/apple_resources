

- Create ML
- MLActionClassifier
-  MLActionClassifier.ModelParameters 

Structure

# MLActionClassifier.ModelParameters

Parameters that affect the training process of an action classifier.

macOS 11.0+

``` source
struct ModelParameters
```

## Topics

### Creating action classifier parameters

init(validation: MLActionClassifier.ModelParameters.ValidationData, batchSize: Int, maximumIterations: Int, predictionWindowSize: Int, augmentationOptions: MLActionClassifier.VideoAugmentationOptions, algorithm: MLActionClassifier.ModelParameters.ModelAlgorithmType, targetFrameRate: Double)

Creates a new set of training parameters for an action classifier with the validation dataset.

### Accessing the training parameters

var maximumIterations: Int

The largest number of training iterations the training session can use.

var batchSize: Int

The number of videos the training session uses for each of its training iterations.

var targetFrameRate: Double

The number of frames the training session uses per second of video to train an action classifier.

var predictionWindowSize: Int

The number of frames the training session uses to train an action classifier.

var algorithm: MLActionClassifier.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to train the action classifier.

var augmentationOptions: MLActionClassifier.VideoAugmentationOptions

The variations the training session uses to generate more variety in the training dataset.

var validation: MLActionClassifier.ModelParameters.ValidationData

The action classifier’s validation dataset.

### Describing the model parameters

var description: String

A text representation of the model parameters.

var debugDescription: String

A text representation of the model parameters that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters shown in a playground.

### Supporting types

enum ValidationData

The source of a validation dataset for an action classifier.

struct VideoAugmentationOptions

The video augmentations for an action classifier training session.

enum ModelAlgorithmType

The action classifier training algorithm options.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible

## See Also

### Supporting types

enum DataSource

A data source for an action classifier.

