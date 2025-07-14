

- Create ML
- MLHandPoseClassifier
-  init(trainingData:parameters:) 

Initializer

# init(trainingData:parameters:)

Creates a hand pose classifier by starting a synchronous training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
init(
    trainingData: MLHandPoseClassifier.DataSource,
    parameters: MLHandPoseClassifier.ModelParameters = ModelParameters()
) throws
```

## Parameters 

`trainingData`  

An MLHandPoseClassifier.DataSource instance.

