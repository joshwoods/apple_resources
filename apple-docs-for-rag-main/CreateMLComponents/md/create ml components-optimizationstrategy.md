

- Create ML Components
-  OptimizationStrategy 

Enumeration

# OptimizationStrategy

A linear optimization strategy.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
enum OptimizationStrategy
```

## Topics

### Optimization strategies

case automatic

Chooses the best optimization strategy based on the problem size and configuration.

case fast

An optimization strategy that minimizes computation time.

case lowMemory

An optimization strategy that minimizes memory use.

case nonSmooth

An optimization strategy that can handle non-smooth problems.

### Creating an optimization strategy

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Operators

static func == (OptimizationStrategy, OptimizationStrategy) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

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

struct FullyConnectedNetworkRegressorModel

A regressor model that uses a fully connected network.

struct BoostedTreeRegressor

A gradient boosted decision tree regressor.

struct TreeRegressorModel

A trained tree regressor model.

