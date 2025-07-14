

- Create ML Components
- MultivariateLinearRegressor
-  MultivariateLinearRegressor.Model 

Structure

# MultivariateLinearRegressor.Model

A trained multivariate linear regressor model.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Model
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Overview

Note

Only `Float` and `Double` are currently supported as the Scalar type.

## Topics

### Creating a regressor model

init(weight: MLShapedArray&lt;Scalar>, bias: MLShapedArray&lt;Scalar>?)

Creates a multivariate linear regressor.

### Getting the properties

var inputSize: Int

The input size.

var outputSize: Int

The output size.

var weight: MLShapedArray&lt;Scalar>

The linear coefficients.

var bias: MLShapedArray&lt;Scalar>?

The bias coefficients.

### Performing the regression

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> MLShapedArray&lt;Scalar>

Performs a prediction on a shaped array.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

Transformer Implementations

## Relationships

### Conforms To

- Sendable
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

