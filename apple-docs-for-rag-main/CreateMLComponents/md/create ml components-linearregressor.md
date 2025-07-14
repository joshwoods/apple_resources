

- Create ML Components
-  LinearRegressor 

Structure

# LinearRegressor

A linear regressor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct LinearRegressor where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint
```

## Topics

### Creating a regressor

init(configuration: LinearRegressor&lt;Scalar>.Configuration)

Creates a linear regressor.

struct Configuration

A linear regressor configuration.

### Getting the configuration

var configuration: LinearRegressor&lt;Scalar>.Configuration

The linear regressor configuration.

### Encoding and decoding

func encode(LinearRegressorModel&lt;Scalar>, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> LinearRegressorModel&lt;Scalar>

Decodes a previously fitted transformer.

### Fitting

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> LinearRegressorModel&lt;Scalar>

Fits a linear regressor model to a sequence of examples.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> LinearRegressorModel&lt;Scalar>

Fits a linear regressor model to a sequence of examples.

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
- UpdatableSupervisedEstimator

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## See Also

### Regressors

protocol Regressor

A transformer that predicts a float value.

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

