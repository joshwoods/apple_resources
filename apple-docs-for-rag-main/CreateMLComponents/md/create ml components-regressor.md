

- Create ML Components
-  Regressor 

Protocol

# Regressor

A transformer that predicts a float value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol Regressor : Transformer where Self.Output : FloatingPoint
```

## Topics

### Performing the prediction

func prediction(from: Self.Input) async throws -> Self.Output

Performs a prediction from a single input.

func prediction&lt;S>(from: S) async throws -> [Self.Output]

Performs a prediction from a sequence of inputs.

## Relationships

### Inherits From

- Transformer

### Conforming Types

- FullyConnectedNetworkRegressorModel
- LinearRegressorModel
- MLModelRegressorAdaptor

## See Also

### Regressors

struct LinearRegressor

A linear regressor.

struct LinearRegressorModel

A trained linear regressor model.

struct MultivariateLinearRegressor

A multivariate linear regressor.

struct MultivariateLinearRegressorConfiguration

A linear regressor configuration.

struct Model

A trained multivariate linear regressor model.

struct FullyConnectedNetworkRegressor

A regressor that uses a fully connected network.

struct FullyConnectedNetworkRegressorModel

A regressor model that uses a fully connected network.

struct BoostedTreeRegressor

A gradient boosted decision tree regressor.

struct TreeRegressorModel

A trained tree regressor model.

enum OptimizationStrategy

A linear optimization strategy.

