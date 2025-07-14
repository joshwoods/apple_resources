

- Create ML Components
-  MultivariateLinearRegressorConfiguration 

Structure

# MultivariateLinearRegressorConfiguration

A linear regressor configuration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct MultivariateLinearRegressorConfiguration
```

## Topics

### Creating a configuration

init()

Creates a default linear regressor configuration.

### Getting the properties

var batchSize: Int

The number of examples in each training batch.

var maximumIterationCount: Int

The maximum number of allowed passes through the data.

var earlyStoppingTolerance: Float

The early-stopping tolerance.

var earlyStoppingIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var learningRate: Float

The optimizer learning rate.

var randomSeed: Int?

A seed to generate reproducible results from random operations.

### Operators

static func == (MultivariateLinearRegressorConfiguration, MultivariateLinearRegressorConfiguration) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

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

