

- Create ML Components
- LinearRegressor
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a linear regressor model to a sequence of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: Input,
    validateOn validation: Validation,
    eventHandler: EventHandler? = nil
) async throws -> LinearRegressorModel where Input : Sequence, Validation : Sequence, Input.Element == AnnotatedFeature, Scalar>, Validation.Element == AnnotatedFeature, Scalar>
```

## Parameters 

`input`  

A sequence of examples used for fitting the regressor.

`validation`  

A sequence of examples used for validating the fitted regressor.

`eventHandler`  

An event handler. This method reports maximum error and root-mean-square error metrics.

## Return Value

The fitted linear regressor model.

## See Also

### Fitting

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> LinearRegressorModel&lt;Scalar>

Fits a linear regressor model to a sequence of examples.

typealias Annotation

The annotation type.

typealias Transformer

The transformer type created by this estimator.

