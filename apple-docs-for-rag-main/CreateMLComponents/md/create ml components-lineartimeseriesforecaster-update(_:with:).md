

- Create ML Components
- LinearTimeSeriesForecaster
-  update(\_:with:) 

Instance Method

# update(\_:with:)

Updates a model with a new batch of examples.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func update(
    _ model: inout LinearTimeSeriesForecaster.Transformer,
    with input: AnnotatedBatch
) async throws -> Scalar
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`model`  

The model to update.

`input`  

A shaped array of windowed features. The shape should be `[batchSize, inputWindowSize, featureSize]`.

## Discussion

Use TimeSeriesForecasterBatches to convert a shaped array of features into batches of windowed features and annotations. Here is an example of training a forecaster:

```
let estimator = LinearTimeSeriesForecaster(configuration: configuration)
var model = estimator.makeTransformer()

let batches = try TimeSeriesForecasterBatches(
    features: features,       // shape [N, featureSize]
    annotations: annotations, // shape [N, annotationSize]
    batchSize: 32,
    inputWindowSize: configuration.inputWindowSize,
    forecastWindowSize: configuration.forecastWindowSize,
    shufflesBatches: true
)

for iteration in 0 ..

