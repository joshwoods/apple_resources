

- Create ML
- MLHandPoseClassifier
-  modelParameters 

Instance Property

# modelParameters

The hand pose model’s configuration parameters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
let modelParameters: MLHandPoseClassifier.ModelParameters
```

## Discussion

The property reflects the model parameters you provide to one of these methods that train a hand pose classifier:

- 

## ``doc://com.apple.CreateML/documentation/CreateML/MLHandPoseClassifier/train(trainingData:parameters:sessionParameters:)``

makeTrainingSession(trainingData:parameters:sessionParameters:)

- init(trainingData:parameters:)

## See Also

### Inspecting a hand pose classifier model

var model: MLModel

The underlying Core ML model of the hand pose classifier stored in memory.

