

- Create ML Components
- MultivariateLinearRegressor
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a model with a new sequence of examples.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func update(
    _ model: inout MultivariateLinearRegressor.Model,
    with input: some Sequence, MLShapedArray>>,
    eventHandler: EventHandler? = nil
) async throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`model`  

A model to update.

`input`  

A sequence of examples. For faster updates, consider passing a single AnnotatedBatch with shaped arrays that contain multiple training examples. For example instead of passing a sequence of `N` shaped arrays with shape `[M]`, pass a single shaped array with shape `[N, M]`. See also update(_:with:).

`eventHandler`  

An event handler. This method reports the mean squared error.

## See Also

### Fitting Progressively

func makeTransformer() -> MultivariateLinearRegressor&lt;Scalar>.Model

Creates a default-initialized model suitable for incremental fitting.

func update(inout MultivariateLinearRegressor&lt;Scalar>.Model, with: AnnotatedBatch&lt;Scalar>) async throws -> Scalar

Updates a model with a new shaped array of examples.

