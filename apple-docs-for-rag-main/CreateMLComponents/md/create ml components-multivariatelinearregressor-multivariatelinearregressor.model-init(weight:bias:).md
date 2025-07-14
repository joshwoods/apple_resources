

- Create ML Components
- MultivariateLinearRegressor
- MultivariateLinearRegressor.Model
-  init(weight:bias:) 

Initializer

# init(weight:bias:)

Creates a multivariate linear regressor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    weight: MLShapedArray,
    bias: MLShapedArray?
)
```

## Parameters 

`weight`  

A shaped array of linear weights.

`bias`  

A one-dimensional shaped array of biases.

