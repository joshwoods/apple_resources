

- Create ML Components
-  FullyConnectedNetworkClassifier 

Structure

# FullyConnectedNetworkClassifier

A classifier that uses a fully connected network.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct FullyConnectedNetworkClassifier where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint, Label : Comparable, Label : Decodable, Label : Encodable, Label : Hashable
```

## Mentioned in 

Creating a multi-label image classifier

## Topics

### Creating the classifier

init(labels: Set&lt;Label>, configuration: FullyConnectedNetworkConfiguration)

Creates a fully connected network classifier.

### Getting the properties

var labels: Set&lt;Label>

The set of possible labels.

var configuration: FullyConnectedNetworkConfiguration

The fully-connected-network configuration.

### Encoding and decoding

func encode(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted encodable transformer.

func decode(from: inout any EstimatorDecoder) throws -> FullyConnectedNetworkClassifierModel&lt;Scalar, Label>

Decodes the estimator.

### Fitting a classifier

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkClassifierModel&lt;Scalar, Label>

Fits a fully connected network classifier model to a sequence of examples.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkClassifierModel&lt;Scalar, Label>

Fits a fully connected network classifier model to a sequence of examples.

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

struct LogisticRegressionClassifier

A logistic regression classifier.

struct LogisticRegressionClassifierModel

A trained logistic regression classifier model.

struct BoostedTreeClassifier

A gradient boosted decision tree classifier.

struct BoostedTreeConfiguration

A boosted tree configuration.

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

