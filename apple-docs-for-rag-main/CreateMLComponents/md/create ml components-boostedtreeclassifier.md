

- Create ML Components
-  BoostedTreeClassifier 

Structure

# BoostedTreeClassifier

A gradient boosted decision tree classifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct BoostedTreeClassifier where Label : Comparable, Label : Decodable, Label : Encodable, Label : Hashable
```

## Topics

### Creating a classifier

init(labels: Set&lt;Label?>, annotationColumnName: String, featureColumnNames: [String], configuration: BoostedTreeConfiguration)

Creates a boosted tree classifier.

### Getting the properties

var annotationColumnID: ColumnID&lt;Label>

The annotation column identifier.

var featureColumnNames: [String]

The names of the columns containing feature values.

var configuration: BoostedTreeConfiguration

Boosted tree configuration.

var labels: Set&lt;Label?>

The set of possible labels.

### Fitting the classifier

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> TreeClassifierModel&lt;Label>

Fits a boosted tree classifier model to a collection of examples.

typealias Annotation

The annotation type.

typealias Transformer

The transformer type created by this estimator.

### Encoding and decoding the classifier

func encode(TreeClassifierModel&lt;Label>, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func encodeLabels(some Collection&lt;Optional&lt;Label>>) throws -> (labels: [String?], encoded: [Int])

func decode(from: inout any EstimatorDecoder) throws -> TreeClassifierModel&lt;Label>

Decodes a previously fitted transformer.

### Default Implementations

SupervisedTabularEstimator Implementations

UpdatableSupervisedTabularEstimator Implementations

## Relationships

### Conforms To

- Copyable
- Sendable
- SupervisedTabularEstimator
- UpdatableSupervisedTabularEstimator

  Conforms when `Label` conforms to `Comparable`, `Decodable`, `Encodable`, and `Hashable`.

## See Also

### Classifiers

protocol Classifier

An estimator that predicts classification probabilities.

struct LogisticRegressionClassifier

A logistic regression classifier.

struct LogisticRegressionClassifierModel

A trained logistic regression classifier model.

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

