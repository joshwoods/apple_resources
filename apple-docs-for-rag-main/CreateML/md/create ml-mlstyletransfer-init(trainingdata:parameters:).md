

- Create ML
- MLStyleTransfer
-  init(trainingData:parameters:) 

Initializer

# init(trainingData:parameters:)

Creates a style transfer model with a training dataset represented by a data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
init(
    trainingData: MLStyleTransfer.DataSource,
    parameters: MLStyleTransfer.ModelParameters = .init()
) throws
```

## Discussion

- trainingData: A style image and a content image, represented by a data source.

