

- Create ML Components
-  BoostedTreeRegressor 

Structure

# BoostedTreeRegressor

A gradient boosted decision tree regressor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct BoostedTreeRegressor
```

## Topics

### Creating a regressor

init(annotationColumnName: String, featureColumnNames: [String], configuration: BoostedTreeConfiguration)

Creates a boosted tree regressor.

### Getting the properties

var annotationColumnID: ColumnID&lt;Annotation>

The annotation column identifier.

var configuration: BoostedTreeConfiguration

Boosted tree configuration.

var featureColumnNames: [String]

The names of the columns containing feature values.

### Fitting a regressor model

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> TreeRegressorModel

Fits a boosted tree regressor model to a collection of examples.

typealias Transformer

The transformer type created by this estimator.

### Encoding and decoding a regressor

func encode(TreeRegressorModel, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> TreeRegressorModel

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

  Conforms when `Annotation` conforms to `Copyable` and `Escapable`.

## See Also

### Regressors

protocol Regressor

A transformer that predicts a float value.

struct LinearRegressor

A linear regressor.

struct LinearRegressorModel

A trained linear regressor model.

struct MultivariateLinearRegressor

A multivariate linear regressor.

struct MultivariateLinearRegressorConfiguration

A linear regressor configuration.

struct Model

A trained multivariate linear regressor model.

struct FullyConnectedNetworkRegressor

A regressor that uses a fully connected network.

struct FullyConnectedNetworkRegressorModel

A regressor model that uses a fully connected network.

struct TreeRegressorModel

A trained tree regressor model.

enum OptimizationStrategy

A linear optimization strategy.

