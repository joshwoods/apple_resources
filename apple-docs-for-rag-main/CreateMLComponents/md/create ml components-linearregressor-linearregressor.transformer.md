

- Create ML Components
- LinearRegressor
-  LinearRegressor.Transformer 

Type Alias

# LinearRegressor.Transformer

The transformer type created by this estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Transformer = LinearRegressorModel
```

## See Also

### Fitting

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> LinearRegressorModel&lt;Scalar>

Fits a linear regressor model to a sequence of examples.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> LinearRegressorModel&lt;Scalar>

Fits a linear regressor model to a sequence of examples.

typealias Annotation

The annotation type.

