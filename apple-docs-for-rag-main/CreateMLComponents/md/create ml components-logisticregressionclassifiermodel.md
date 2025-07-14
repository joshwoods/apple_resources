

- Create ML Components
-  LogisticRegressionClassifierModel 

Structure

# LogisticRegressionClassifierModel

A trained logistic regression classifier model.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct LogisticRegressionClassifierModel where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint, Label : Comparable, Label : Decodable, Label : Encodable, Label : Hashable
```

## Topics

### Creating a regression model

init(coefficients: some Sequence&lt;Scalar>, labels: Set&lt;Label>)

Creates a logistic regression model.

### Getting the properties

var coefficients: [Scalar]

The linear coefficients.

var featureCount: Int

The number of features expected in the input.

### Performing the classification

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> ClassificationDistribution&lt;Label>

Performs a classification on a single input.

typealias Input

The input type.

### Type Aliases

typealias Output

The output type.

### Default Implementations

Transformer Implementations

## Relationships

### Conforms To

- Classifier
- Sendable
- Transformer

## See Also

### Classifiers

protocol Classifier

An estimator that predicts classification probabilities.

struct LogisticRegressionClassifier

A logistic regression classifier.

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

struct TimeSeriesClassifierConfiguration

The configuration for a time-series classifier.

