

- Create ML Components
-  FullyConnectedNetworkConfiguration 

Structure

# FullyConnectedNetworkConfiguration

A fully connected network configuration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct FullyConnectedNetworkConfiguration
```

## Topics

### Creating a network configuration

init()

Creates a default fully-connected-network configuration.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Getting the properties

var batchSize: Int

The number of examples to use per mini-batch.

var dropoutProbability: Float

The dropout probability.

var earlyStopIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var earlyStoppingTolerance: Double

The early-stopping tolerance.

var hiddenUnitCounts: [Int]

The number of neurons in each hidden layer.

var learningRate: Float

The learning rate.

var maximumIterations: Int

The maximum number of iterations.

var randomSeed: Int

A seed to generate reproducible results from random operations such as column and row subsampling.

### Operators

static func == (FullyConnectedNetworkConfiguration, FullyConnectedNetworkConfiguration) -> Bool

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

### Classifiers

protocol Classifier

An estimator that predicts classification probabilities.

struct LogisticRegressionClassifier

A logistic regression classifier.

struct LogisticRegressionClassifierModel

A trained logistic regression classifier model.

struct BoostedTreeClassifier

A gradient boosted decision tree classifier.

struct BoostedTreeConfiguration

A boosted tree configuration.

struct FullyConnectedNetworkClassifier

A classifier that uses a fully connected network.

struct FullyConnectedNetworkClassifierModel

A classifier model that uses a fully connected network.

struct FullyConnectedNetworkMultiLabelClassifier

A classifier that uses a multi-label fully-connected network.

struct FullyConnectedNetworkMultiLabelClassifierModel

A multi-label classifier model that uses a fully-connected network.

struct TreeClassifierModel

A trained tree classifier model.

struct TimeSeriesClassifier

struct TimeSeriesClassifierConfiguration

The configuration for a time-series classifier.

