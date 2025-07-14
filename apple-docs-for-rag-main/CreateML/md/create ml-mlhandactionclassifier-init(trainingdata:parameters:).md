

- Create ML
- MLHandActionClassifier
-  init(trainingData:parameters:) 

Initializer

# init(trainingData:parameters:)

Creates a hand action classifier by starting a synchronous training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
init(
    trainingData: MLHandActionClassifier.DataSource,
    parameters: MLHandActionClassifier.ModelParameters = ModelParameters()
) throws
```

## Parameters 

`trainingData`  

An MLHandActionClassifier.DataSource instance.

`parameters`  

An MLHandActionClassifier.ModelParameters instance you use to configure the model for the training session.

