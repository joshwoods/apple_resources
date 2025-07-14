

- Create ML Components
-  FullyConnectedNetworkRegressor 

Structure

# FullyConnectedNetworkRegressor

A regressor that uses a fully connected network.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct FullyConnectedNetworkRegressor where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint
```

## Topics

### Creating the regressor

init(configuration: FullyConnectedNetworkConfiguration)

Creates a fully connected network regressor.

### Getting the configuration

var configuration: FullyConnectedNetworkConfiguration

The fully-connected-network configuration.

### Decoding a regressor

func decode(from: inout any EstimatorDecoder) throws -> FullyConnectedNetworkRegressorModel&lt;Scalar>

Decodes the estimator.

### Fitting a regressor

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkRegressor&lt;Scalar>.Transformer

Fits a fully connected network regressor model to a sequence of examples.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkRegressorModel&lt;Scalar>

Fits a fully connected network regressor model to a sequence of examples.

typealias Annotation

The annotation type.

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

SupervisedEstimator Implementations

UpdatableSupervisedEstimator Implementations

## Relationships

### Conforms To

- Copyable
- Sendable
- SupervisedEstimator

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- UpdatableSupervisedEstimator

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## See Also

### Regressors

protocol Regressor

A transformer that predicts a float value.

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

struct FullyConnectedNetworkRegressorModel

A regressor model that uses a fully connected network.

struct BoostedTreeRegressor

A gradient boosted decision tree regressor.

struct TreeRegressorModel

A trained tree regressor model.

enum OptimizationStrategy

A linear optimization strategy.

