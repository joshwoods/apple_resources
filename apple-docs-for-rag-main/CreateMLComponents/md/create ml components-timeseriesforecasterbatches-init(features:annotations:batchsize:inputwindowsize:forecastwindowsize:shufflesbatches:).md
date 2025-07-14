

- Create ML Components
- TimeSeriesForecasterBatches
-  init(features:annotations:batchSize:inputWindowSize:forecastWindowSize:shufflesBatches:) 

Initializer

# init(features:annotations:batchSize:inputWindowSize:forecastWindowSize:shufflesBatches:)

Creates a batch sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    features: MLShapedArray,
    annotations: MLShapedArray,
    batchSize: Int,
    inputWindowSize: Int,
    forecastWindowSize: Int,
    shufflesBatches: Bool = true
) throws
```

## Parameters 

`features`  

A shaped array of features, it must have two dimensions.

`annotations`  

A shaped array of annotations, it must have two dimensions.

`batchSize`  

The batch size. Must be positive.

`inputWindowSize`  

The number of input samples. Must be positive.

`forecastWindowSize`  

The number of prediction samples. Must be positive.

`shufflesBatches`  

A Boolean value indicating whether to shuffle the batches.

