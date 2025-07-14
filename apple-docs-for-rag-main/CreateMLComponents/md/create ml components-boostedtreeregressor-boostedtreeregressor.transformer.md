

- Create ML Components
- BoostedTreeRegressor
-  BoostedTreeRegressor.Transformer 

Type Alias

# BoostedTreeRegressor.Transformer

The transformer type created by this estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Transformer = TreeRegressorModel
```

## See Also

### Fitting a regressor model

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> TreeRegressorModel

Fits a boosted tree regressor model to a collection of examples.

