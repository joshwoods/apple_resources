

- Create ML Components
- MultivariateLinearRegressor
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a linear regressor model to a sequence of annotated features.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func fitted(
    to input: some Sequence, MLShapedArray>>,
    validateOn validation: some Sequence, MLShapedArray>>,
    eventHandler: EventHandler? = nil
) async throws -> MultivariateLinearRegressor.Model
```

## Parameters 

`input`  

A sequence of examples used for fitting the regressor. For faster processing, instead of passing a sequence of shaped arrays, consider passing a single shaped array containing all the training examples. For example instead of passing `N` shaped arrays with shape `[M]`, pass a single shaped array with shape `[N, M]`. See fitted(to:validateOn:eventHandler:).

`validation`  

A sequence of examples used for validating the fitted regressor.

`eventHandler`  

An event handler. This method reports mean squared errors.

## Return Value

The fitted linear regressor model.

## See Also

### Fitting

func fitted(to: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Fits a linear regressor model to a sequence of annotated features.

func fitted(to: AnnotatedBatch&lt;Scalar>, validateOn: AnnotatedBatch&lt;Scalar>?, eventHandler: EventHandler?) async throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Fits a linear regressor model to shaped arrays of features and annotations.

