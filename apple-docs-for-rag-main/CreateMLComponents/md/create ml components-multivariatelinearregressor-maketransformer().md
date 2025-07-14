

- Create ML Components
- MultivariateLinearRegressor
-  makeTransformer() 

Instance Method

# makeTransformer()

Creates a default-initialized model suitable for incremental fitting.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func makeTransformer() -> MultivariateLinearRegressor.Model
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## See Also

### Fitting Progressively

func update(inout MultivariateLinearRegressor&lt;Scalar>.Model, with: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws

Updates a model with a new sequence of examples.

func update(inout MultivariateLinearRegressor&lt;Scalar>.Model, with: AnnotatedBatch&lt;Scalar>) async throws -> Scalar

Updates a model with a new shaped array of examples.

