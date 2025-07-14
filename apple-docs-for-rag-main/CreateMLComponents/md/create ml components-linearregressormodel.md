

- Create ML Components
-  LinearRegressorModel 

Structure

# LinearRegressorModel

A trained linear regressor model.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct LinearRegressorModel where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint
```

## Topics

### Creating a regressor model

init(coefficients: some Sequence&lt;Scalar>)

Creates a linear regression model.

### Getting the properties

var featureCount: Int

The number of features expected in the input.

var coefficients: [Scalar]

The linear coefficients.

### Performing the regression

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> Scalar

Performs a regression on a single input.

typealias Input

The input type.

### Type Aliases

typealias Output

The output type.

### Default Implementations

Regressor Implementations

Transformer Implementations

## Relationships

### Conforms To

- Regressor
- Sendable
- Transformer

## See Also

### Regressors

protocol Regressor

A transformer that predicts a float value.

struct LinearRegressor

A linear regressor.

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

