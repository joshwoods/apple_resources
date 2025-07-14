

- Create ML Components
-  LogisticRegressionClassifier 

Structure

# LogisticRegressionClassifier

A logistic regression classifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct LogisticRegressionClassifier where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint, Label : Comparable, Label : Decodable, Label : Encodable, Label : Hashable
```

## Topics

### Creating a classifier

init(labels: Set&lt;Label>, configuration: LogisticRegressionClassifier&lt;Scalar, Label>.Configuration)

Creates a logistic regression classifier.

struct Configuration

A logistic regression classifier configuration.

### Getting the properties

var configuration: LogisticRegressionClassifier&lt;Scalar, Label>.Configuration

The logistic regression classifier configuration.

var labels: Set&lt;Label>

The set of possible labels.

### Encoding and decoding

func encode(LogisticRegressionClassifierModel&lt;Scalar, Label>, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> LogisticRegressionClassifierModel&lt;Scalar, Label>

Decodes a previously fitted transformer.

### Fitting

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> LogisticRegressionClassifier&lt;Scalar, Label>.Transformer

Fits a logistic regression classifier model to a sequence of examples while validating with a validation sequence.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> LogisticRegressionClassifierModel&lt;Scalar, Label>

Fits a logistic regression classifier model to a sequence of examples.

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

  Conforms when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## See Also

### Classifiers

protocol Classifier

An estimator that predicts classification probabilities.

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

struct TimeSeriesClassifierConfiguration

The configuration for a time-series classifier.

