

- Create ML Components
-  FullyConnectedNetworkRegressorModel 

Structure

# FullyConnectedNetworkRegressorModel

A regressor model that uses a fully connected network.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct FullyConnectedNetworkRegressorModel where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint
```

## Topics

### Creating a regressor model

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Performing a regression

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkRegressorModel&lt;Scalar>.Target

Performs regression on a shaped array.

typealias Target

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Regressor Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Regressor
- Transformer

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

struct FullyConnectedNetworkRegressor

A regressor that uses a fully connected network.

struct BoostedTreeRegressor

A gradient boosted decision tree regressor.

struct TreeRegressorModel

A trained tree regressor model.

enum OptimizationStrategy

A linear optimization strategy.

