

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
-  init(validationData:batchSize:maxIterations:) Deprecated

Initializer

# init(validationData:batchSize:maxIterations:)

Creates a model parameters instance for an object-detector training session set to use the full network algorithm.

macOS 10.15–11.0Deprecated

``` source
init(
    validationData: MLObjectDetector.DataSource,
    batchSize: Int? = nil,
    maxIterations: Int? = nil
) throws
```

## Discussion

- validationData: An MLObjectDetector.ModelParameters.ValidationData instance that contains your validation dataset.

- batchSize: The number of images the object detector uses for each training iteration. If you don’t have a preference, set this parameter to `nil` to tell Create ML to use an appropriate value when it trains the model.

- maxIterations: The largest number of training iterations the object detector can use. If you don’t have a preference, set this parameter to `nil` to tell Create ML to use an appropriate value when it trains the model.

## See Also

### Creating object detector parameters

init(validation: MLObjectDetector.ModelParameters.ValidationData, batchSize: Int?, maxIterations: Int?)

Creates a model parameters instance for an object-detector training session set to use the full network algorithm.

init(validation: MLObjectDetector.ModelParameters.ValidationData, batchSize: Int?, maxIterations: Int?, gridSize: CGSize, algorithm: MLObjectDetector.ModelParameters.ModelAlgorithmType)

Creates a model parameters instance for an object-detector training session.

