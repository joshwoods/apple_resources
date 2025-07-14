

- Create ML Components
-  FullyConnectedNetworkMultiLabelClassifierModel 

Structure

# FullyConnectedNetworkMultiLabelClassifierModel

A multi-label classifier model that uses a fully-connected network.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct FullyConnectedNetworkMultiLabelClassifierModel where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint, Label : Comparable, Label : Decodable, Label : Encodable, Label : Hashable
```

## Topics

### Performing a classification

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) throws -> ClassificationDistribution&lt;Label>

Performs a classification on a shaped array.

### Computing evaluation metrics

func evaluation(on: some Collection&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, Set&lt;Label>>>, confidenceThresholds: [Label : Float]) throws -> MultiLabelClassificationMetrics&lt;Label>

Computes evaluation metrics on annotated examples.

### Performing a prediction

func prediction&lt;S>(from: S, confidenceThresholds: [Label : Scalar]) throws -> [ClassificationDistribution&lt;Label>]

Performs a sequence of predictions and keeps label-confidence pairs that are greater than or equal to the provided confidence thresholds.

func prediction(from: FullyConnectedNetworkMultiLabelClassifierModel&lt;Scalar, Label>.Input, confidenceThresholds: [Label : Scalar]) throws -> ClassificationDistribution&lt;Label>

Performs a prediction and keeps label-confidence pairs that are greater than or equal to the provided confidence thresholds.

### Updating the precision recall curve

func updatePrecisionRecallCurves(some Collection&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, Set&lt;Label>>>) async throws

Updates the per-label precision-recall curve using the input data.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Sendable
- Transformer

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

struct FullyConnectedNetworkConfiguration

A fully connected network configuration.

struct TreeClassifierModel

A trained tree classifier model.

struct TimeSeriesClassifier

struct TimeSeriesClassifierConfiguration

The configuration for a time-series classifier.

