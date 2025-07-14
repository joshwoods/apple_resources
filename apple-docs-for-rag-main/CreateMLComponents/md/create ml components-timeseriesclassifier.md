

- Create ML Components
-  TimeSeriesClassifier 

Structure

# TimeSeriesClassifier

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct TimeSeriesClassifier where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint, Label : Comparable, Label : Decodable, Label : Encodable, Label : Hashable
```

## Topics

### Structures

struct Model

A time-series classifier model.

### Initializers

init(labels: Set&lt;Label>, configuration: TimeSeriesClassifierConfiguration)

Creates a time series classifier.

### Instance Properties

var configuration: TimeSeriesClassifierConfiguration

The configuration.

var labels: Set&lt;Label>

The set of possible labels.

### Instance Methods

func fitted(to: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, Label>>, eventHandler: EventHandler?) async throws -> TimeSeriesClassifier&lt;Scalar, Label>.Model

Fits a time series classifier model to a sequence of examples.

func fitted(to: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, Label>>, validateOn: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, Label>>, eventHandler: EventHandler?) async throws -> TimeSeriesClassifier&lt;Scalar, Label>.Model

Fits a time series classifier model to a sequence of examples.

### Type Aliases

typealias Annotation

The annotation type.

typealias Configuration

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

  Conforms when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

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

struct TimeSeriesClassifierConfiguration

The configuration for a time-series classifier.

