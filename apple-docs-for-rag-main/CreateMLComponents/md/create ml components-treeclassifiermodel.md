

- Create ML Components
-  TreeClassifierModel 

Structure

# TreeClassifierModel

A trained tree classifier model.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct TreeClassifierModel where Label : Hashable
```

## Topics

### Getting the properties

var classCount: Int

The number of classes.

var featureColumnNames: [String]

The names of the columns containing feature values.

var predictionColumnName: String

The name of the column containing the predicted labels.

### Building a data frame

func buildDataFrame([ClassificationDistribution&lt;Label>]) -> DataFrame

Builds a data frame containing a labels column and a probability distribution column.

### Applying

func applied(to: DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Performs a classification on a data frame.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

TabularTransformer Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Sendable
- TabularTransformer
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

struct FullyConnectedNetworkMultiLabelClassifierModel

A multi-label classifier model that uses a fully-connected network.

struct FullyConnectedNetworkConfiguration

A fully connected network configuration.

struct TimeSeriesClassifier

struct TimeSeriesClassifierConfiguration

The configuration for a time-series classifier.

