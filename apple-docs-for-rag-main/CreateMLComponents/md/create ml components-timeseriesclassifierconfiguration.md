

- Create ML Components
-  TimeSeriesClassifierConfiguration 

Structure

# TimeSeriesClassifierConfiguration

The configuration for a time-series classifier.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct TimeSeriesClassifierConfiguration
```

## Topics

### Operators

static func == (TimeSeriesClassifierConfiguration, TimeSeriesClassifierConfiguration) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

Creates a configuration.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var batchSize: Int

The number of examples in each training batch.

var earlyStoppingIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var earlyStoppingTolerance: Float

The early-stopping tolerance.

var hashValue: Int

The hash value.

var learningRate: Float

The starting learning rate.

var maximumIterationCount: Int

The maximum number of allowed passes through the data.

var maximumSequenceLength: Int

The maximum number of samples that can be classified.

var minimumSequenceLength: Int

The minimum number of samples required to produce a classification.

var randomSeed: Int?

A seed to generate reproducible results from random operations.

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

struct FullyConnectedNetworkConfiguration

A fully connected network configuration.

struct TreeClassifierModel

A trained tree classifier model.

struct TimeSeriesClassifier

