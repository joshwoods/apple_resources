

- Create ML Components
- MultivariateLinearRegressor
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a linear regressor model to shaped arrays of features and annotations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func fitted(
    to input: AnnotatedBatch,
    validateOn validation: AnnotatedBatch?,
    eventHandler: EventHandler? = nil
) async throws -> MultivariateLinearRegressor.Model
```

## Parameters 

`input`  

An annotated batch containing the features and annotations. The last dimension of the features is the model’s input size and the last dimension of the annotations is the model’s output size. All the leading dimensions of the features must match all leading dimensions of the annotations. For example, the feature shape can be `[N, X]` and the annotation shape can be `[N, Y]` for `N` examples where `X` is the input size and `Y` is the output size.

`validation`  

An annotated batch containing the validation features and annotations. The last dimension of the features must be `inputSize` and the last dimension of the annotations must be `outputSize`. All the leading dimensions of the features must match all leading dimensions of the annotations.

`eventHandler`  

An event handler. This method reports the mean squared errors.

## Return Value

The fitted model.

## See Also

### Fitting

func fitted(to: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Fits a linear regressor model to a sequence of annotated features.

func fitted(to: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, validateOn: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Fits a linear regressor model to a sequence of annotated features.

