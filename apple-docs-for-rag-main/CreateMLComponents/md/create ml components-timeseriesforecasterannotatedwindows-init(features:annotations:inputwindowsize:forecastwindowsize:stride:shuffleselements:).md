

- Create ML Components
- TimeSeriesForecasterAnnotatedWindows
-  init(features:annotations:inputWindowSize:forecastWindowSize:stride:shufflesElements:) 

Initializer

# init(features:annotations:inputWindowSize:forecastWindowSize:stride:shufflesElements:)

Creates a batch sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    features: MLShapedArray,
    annotations: MLShapedArray,
    inputWindowSize: Int,
    forecastWindowSize: Int,
    stride: Int = 1,
    shufflesElements: Bool = true
) throws
```

## Parameters 

`features`  

A shaped array of features, it must have two dimensions.

`annotations`  

A shaped array of annotations, it must have two dimensions.

`inputWindowSize`  

The number of input samples. Must be positive.

`forecastWindowSize`  

The number of prediction samples. Must be positive.

`stride`  

The number of samples between windows. Must be positive. Defaults to 1.

`shufflesElements`  

A Boolean value indicating whether to shuffle the elements. Defaults to true.

