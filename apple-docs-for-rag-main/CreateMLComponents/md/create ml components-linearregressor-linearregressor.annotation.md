

- Create ML Components
- LinearRegressor
-  LinearRegressor.Annotation 

Type Alias

# LinearRegressor.Annotation

The annotation type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Annotation = Scalar
```

## See Also

### Fitting

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> LinearRegressorModel&lt;Scalar>

Fits a linear regressor model to a sequence of examples.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> LinearRegressorModel&lt;Scalar>

Fits a linear regressor model to a sequence of examples.

typealias Transformer

The transformer type created by this estimator.

