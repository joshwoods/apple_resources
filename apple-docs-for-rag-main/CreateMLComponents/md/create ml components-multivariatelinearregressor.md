

- Create ML Components
-  MultivariateLinearRegressor 

Structure

# MultivariateLinearRegressor

A multivariate linear regressor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct MultivariateLinearRegressor where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint
```

## Overview

Unlike a LinearRegressor, a MultivariateLinearRegressor supports shaped array outputs with any number of elements. It also provides a wider range of training options better suited for large multi-dimensional regression.

Note

Only `Float` and `Double` are currently supported as the Scalar type. You may get faster training when using `Float`.

## Topics

### Creating a regressor

init(configuration: MultivariateLinearRegressor&lt;Scalar>.Configuration)

Creates a multivariate linear regressor.

### Getting the configuration

var configuration: MultivariateLinearRegressor&lt;Scalar>.Configuration

The linear regressor configuration.

### Fitting

func fitted(to: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Fits a linear regressor model to a sequence of annotated features.

func fitted(to: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, validateOn: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Fits a linear regressor model to a sequence of annotated features.

func fitted(to: AnnotatedBatch&lt;Scalar>, validateOn: AnnotatedBatch&lt;Scalar>?, eventHandler: EventHandler?) async throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Fits a linear regressor model to shaped arrays of features and annotations.

### Fitting Progressively

func makeTransformer() -> MultivariateLinearRegressor&lt;Scalar>.Model

Creates a default-initialized model suitable for incremental fitting.

func update(inout MultivariateLinearRegressor&lt;Scalar>.Model, with: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws

Updates a model with a new sequence of examples.

func update(inout MultivariateLinearRegressor&lt;Scalar>.Model, with: AnnotatedBatch&lt;Scalar>) async throws -> Scalar

Updates a model with a new shaped array of examples.

### Encoding and decoding

func encode(MultivariateLinearRegressor&lt;Scalar>.Model, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Decodes a previously fitted transformer.

func encodeWithOptimizer(MultivariateLinearRegressor&lt;Scalar>.Model, to: inout any EstimatorEncoder) throws

Encodes the model and optimizer to an encoder.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Reads the encoded model and optimizer with a decoder.

### Structures

struct Model

A trained multivariate linear regressor model.

### Type Aliases

typealias Annotation

The annotation type.

typealias Configuration

typealias Feature

The feature type.

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

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- UpdatableSupervisedEstimator

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## See Also

### Regressors

protocol Regressor

A transformer that predicts a float value.

struct LinearRegressor

A linear regressor.

struct LinearRegressorModel

A trained linear regressor model.

struct MultivariateLinearRegressorConfiguration

A linear regressor configuration.

struct Model

A trained multivariate linear regressor model.

struct FullyConnectedNetworkRegressor

A regressor that uses a fully connected network.

struct FullyConnectedNetworkRegressorModel

A regressor model that uses a fully connected network.

struct BoostedTreeRegressor

A gradient boosted decision tree regressor.

struct TreeRegressorModel

A trained tree regressor model.

enum OptimizationStrategy

A linear optimization strategy.

