

- Create ML Components
-  FullyConnectedNetworkMultiLabelClassifier 

Structure

# FullyConnectedNetworkMultiLabelClassifier

A classifier that uses a multi-label fully-connected network.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct FullyConnectedNetworkMultiLabelClassifier where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint, Scalar : Decodable, Scalar : Encodable, Label : Comparable, Label : Decodable, Label : Encodable, Label : Hashable
```

## Mentioned in 

Creating a multi-label image classifier

## Topics

### Creating a classifier

init(labels: Set&lt;Label>, configuration: FullyConnectedNetworkConfiguration)

Creates a full-connected network multi-label classifier.

### Getting the properties

var configuration: FullyConnectedNetworkConfiguration

The fully-connected network configuration.

static var defaultConfiguration: FullyConnectedNetworkConfiguration

The default fully-connected network configration.

var labels: Set&lt;Label>

The set of possible labels.

### Fitting a classifier

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkMultiLabelClassifierModel&lt;Scalar, Label>

Fits a fully-connected network multi-label classifier model to a sequence of examples.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkMultiLabelClassifierModel&lt;Scalar, Label>

Fits a fully-connected network multi-label classifier model to a sequence of examples.

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

  Conforms when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Scalar` conforms to `Decodable`, `Scalar` conforms to `Encodable`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

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

struct FullyConnectedNetworkMultiLabelClassifierModel

A multi-label classifier model that uses a fully-connected network.

struct FullyConnectedNetworkConfiguration

A fully connected network configuration.

struct TreeClassifierModel

A trained tree classifier model.

struct TimeSeriesClassifier

struct TimeSeriesClassifierConfiguration

The configuration for a time-series classifier.

