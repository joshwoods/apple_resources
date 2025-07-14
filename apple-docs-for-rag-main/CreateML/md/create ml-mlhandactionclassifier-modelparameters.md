

- Create ML
- MLHandActionClassifier
-  modelParameters 

Instance Property

# modelParameters

The hand action model’s configuration parameters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
let modelParameters: MLHandActionClassifier.ModelParameters
```

## Discussion

The property reflects the model parameters you provide to one of these methods that train a hand action classifier:

- 

## ``doc://com.apple.CreateML/documentation/CreateML/MLHandActionClassifier/train(trainingData:parameters:sessionParameters:)``

makeTrainingSession(trainingData:parameters:sessionParameters:)

- init(trainingData:parameters:)

## See Also

### Inspecting a hand action classifier model

var model: MLModel

The underlying Core ML model of the hand action classifier stored in memory.

