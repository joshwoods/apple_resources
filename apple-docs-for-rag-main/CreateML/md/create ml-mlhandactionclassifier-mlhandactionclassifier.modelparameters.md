

- Create ML
- MLHandActionClassifier
-  MLHandActionClassifier.ModelParameters 

Structure

# MLHandActionClassifier.ModelParameters

A set of parameters that affect the training process of a hand action classifier task.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
struct ModelParameters
```

## Topics

### Creating hand action model parameters

init(validation: MLHandActionClassifier.ModelParameters.ValidationData, batchSize: Int, maximumIterations: Int, predictionWindowSize: Int, augmentationOptions: MLHandActionClassifier.VideoAugmentationOptions, algorithm: MLHandActionClassifier.ModelParameters.ModelAlgorithmType, targetFrameRate: Double)

Creates a set of training session parameters for a hand action classifier task.

### Accessing hand action training parameters

var maximumIterations: Int

The largest number of training iterations you allow the training session to use.

var batchSize: Int

The number of videos the model training session uses for each training iteration.

var targetFrameRate: Double

The number of video frames per second the hand action classifier model expects as its input at runtime.

var predictionWindowSize: Int

The number of video frames the model training session uses to train a hand action classifier.

var algorithm: MLHandActionClassifier.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to create the hand action classifier.

var augmentationOptions: MLHandActionClassifier.VideoAugmentationOptions

The variations the training session uses to add more variety to its training dataset.

var validation: MLHandActionClassifier.ModelParameters.ValidationData

A dataset the hand action classifier task uses to evaluate the model that’s distinct from the training dataset.

### Describing hand action model parameters

var description: String

A text representation of the hand action parameters.

var debugDescription: String

A text representation of the hand action parameters suitable for debugging.

var playgroundDescription: Any

A description of the hand action parameters that’s viewable in a playground.

### Parameter supporting types

struct VideoAugmentationOptions

Options a hand action classification training session can use to generate additional training data from the videos you provide.

enum ValidationData

A dataset a hand action classifier task uses to validate the model during a training session.

enum ModelAlgorithmType

The hand action classifier training algorithm options.

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

A hand action classifier dataset that contains annotated videos or hand joint location data.

