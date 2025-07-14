

- Create ML Components
- MultivariateLinearRegressor
-  update(\_:with:) 

Instance Method

# update(\_:with:)

Updates a model with a new shaped array of examples.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func update(
    _ model: inout MultivariateLinearRegressor.Model,
    with input: AnnotatedBatch
) async throws -> Scalar
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`model`  

A model to update.

`input`  

An annotated batch containing the features and annotations. The last dimension of the features is the model’s input size and the last dimension of the annotations is the model’s output size. All the leading dimensions of the features must match all leading dimensions of the annotations. For example, the feature shape can be `[N, X]` and the annotation shape can be `[N, Y]` for `N` examples where `X` is the input size and `Y` is the output size.

## Return Value

The mean squared error for the batch, also known as the batch loss.

## See Also

### Fitting Progressively

func makeTransformer() -> MultivariateLinearRegressor&lt;Scalar>.Model

Creates a default-initialized model suitable for incremental fitting.

func update(inout MultivariateLinearRegressor&lt;Scalar>.Model, with: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws

Updates a model with a new sequence of examples.

