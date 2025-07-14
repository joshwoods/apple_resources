

- Create ML Components
-  Transformer 

Protocol

# Transformer

A transformer that takes an input and produces an output.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol Transformer
```

## Topics

### Applying and adapting

func applied(to: Self.Input, eventHandler: EventHandler?) async throws -> Self.Output

Performs the transformation on a single input.

**Required** Default implementations provided.

func adaptedAsAnnotatedFeatureTransformer&lt;Annotation>(annotationType: Annotation.Type) -> some Transformer&lt;AnnotatedFeature&lt;Self.Input, Annotation>, AnnotatedFeature&lt;Self.Output, Annotation>> 

Returns an annotated-feature transformer that transforms the features using this transformer while leaving the annotations unchanged.

func adaptedAsAnnotatedPredictionTransformer&lt;Annotation>(annotationType: Annotation.Type) -> some Transformer&lt;AnnotatedPrediction&lt;Self.Input, Annotation>, AnnotatedPrediction&lt;Self.Output, Annotation>> 

Returns an annotated-prediction transformer that transforms the predictions using this transformer while leaving the annotations unchanged.

func adaptedAsEstimator() -> TransformerToEstimatorAdaptor&lt;Self>

Exposes this transformer as a trivial estimator.

func adaptedAsRandomTransformer() -> some RandomTransformer&lt;Self.Input, Self.Output> 

Returns a random transformer wrapping a transformer.

func adaptedAsUpdatableEstimator() -> TransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this transformer as a trivial estimator.

associatedtype Input

The input type.

**Required**

associatedtype Output

The output type.

**Required**

### Appending

func appending&lt;Other>(Other) -> PreprocessingSupervisedTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableEstimator&lt;Self, Other>

Composes this transformer with an updatable estimator.

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;AnnotatedFeature&lt;Self.Input, Annotation>, Other.Output> 

Composes this transformer with an annotated-feature transformer.

func appending&lt;Other>(Other) -> ComposedTransformer&lt;Self, Other>

Composes this transformer with another transformer.

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;Self.Input, AnnotatedPrediction&lt;Other.Output, Annotation>> 

Composes this transformer with a prediction-only transformer.

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedEstimator&lt;Self, Other>

Composes this transformer with an updatable supervised estimator.

func appending&lt;Other>(Other) -> PreprocessingEstimator&lt;Self, Other>

Composes this transformer with an estimator.

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;Self.Input, AnnotatedFeature&lt;Other.Output, Annotation>> 

Composes this transformer with a feature-only transformer.

func appending&lt;Other, Annotation>(Other) -> some Transformer&lt;AnnotatedPrediction&lt;Self.Input, Annotation>, Other.Output> 

Composes this transformer with an annotated-feature transformer.

func appending&lt;Other>(Other) -> PreprocessingSupervisedEstimator&lt;Self, Other>

Composes this transformer with a supervised estimator.

func appending&lt;Other>(Other) -> PreprocessingUpdatableTemporalEstimator&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;TransformerToTemporalAdaptor&lt;Self>, Other>

Composes this transformer with a temporal transformer.

Deprecated

### Transforming and predicting

func callAsFunction(Self.Input, eventHandler: EventHandler?) async throws -> Self.Output

Performs the transformation on a single input.

func callAsFunction&lt;S>(S, eventHandler: EventHandler?) async throws -> [Self.Output]

Performs the transformation on a sequence of inputs.

func prediction&lt;S, Label>(from: S) async throws -> [ClassificationDistribution&lt;Label>]

Performs a prediction from a sequence of inputs.

func prediction&lt;Label>(from: Self.Input) async throws -> ClassificationDistribution&lt;Label>

Performs a prediction from a single input.

func prediction&lt;S, Annotation>(from: S, eventHandler: EventHandler?) async throws -> [AnnotatedPrediction&lt;Self.Output, Annotation>]

Performs a prediction on a sequence of annotated inputs.

### Exporting

func export(to: URL) throws

Exports this transformer as a CoreML model.

func export(to: URL, metadata: ModelMetadata) throws

Exports this transformer as a CoreML model with userInfo.

### Instance Methods

func adaptedAsTemporal() -> TransformerToTemporalAdaptor&lt;Self>

Exposes this transformer as a temporal transformer.

Deprecated

func adaptedAsTemporal() -> TemporalAdaptor&lt;Self>

Exposes this transformer as a temporal transformer.

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;TemporalAdaptor&lt;Self>, Other>

Composes this transformer with a temporal transformer.

## Relationships

### Inherited By

- Classifier
- ImageFeatureExtractor
- Regressor
- TabularTransformer

### Conforming Types

- AudioConvertingTransformer
- AudioReader
- ColumnConcatenator
- ColumnSelectorTransformer
- ComposedTabularTransformer
- ComposedTransformer
- DateFeatureExtractor
- FullyConnectedNetworkClassifierModel
- FullyConnectedNetworkMultiLabelClassifierModel
- FullyConnectedNetworkRegressorModel
- HumanBodyActionPeriodPredictor
- HumanBodyPoseExtractor
- HumanHandPoseExtractor
- ImageBlur
- ImageColorTransformer
- ImageCropper
- ImageExposureAdjuster
- ImageFeaturePrint
- ImageFlipper
- ImageReader
- ImageRotator
- ImageScaler
- ImputeTransformer
- JointsSelector
- LinearRegressorModel
- LinearTimeSeriesForecaster.Model

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- LinearTransformer
- LogisticRegressionClassifierModel
- MLModelClassifierAdaptor
- MLModelImageFeatureExtractor
- MLModelRegressorAdaptor
- MLModelTransformerAdaptor
- MaxAbsScaler.Transformer

  Conforms when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

- MinMaxScaler.Transformer

  Conforms when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

- MultivariateLinearRegressor.Model

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- NormalizationScaler.Transformer

  Conforms when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

- OneHotEncoder.Transformer

  Conforms when `Category` conforms to `Comparable`, `Decodable`, `Encodable`, and `Hashable`.

- OptionalUnwrapper
- OrdinalEncoder.Transformer

  Conforms when `Category` conforms to `Comparable`, `Decodable`, `Encodable`, and `Hashable`.

- PoseSelector
- RandomImageNoiseGenerator
- Reshaper
- RobustScaler.Transformer

  Conforms when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

- StandardScaler.Transformer

  Conforms when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

- TimeSeriesClassifier.Model

  Conforms when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

- TreeClassifierModel
- TreeRegressorModel
- VideoReader

## See Also

### Protocols

protocol TemporalTransformer

A transformer that takes an asynchronous input sequence of temporal features and produces an asynchronous output sequence.

protocol RandomTransformer

A transformer that takes an input and a random number generator and produces a randomized output.

protocol Estimator

An estimator that creates a transformer by fitting to a data set.

protocol TemporalEstimator

An estimator that creates a transformer by fitting to a sequence of temporal features.

Deprecated

protocol SupervisedEstimator

An estimator that creates a transformer by fitting to a data set.

protocol SupervisedTemporalEstimator

An estimator that creates a transformer by fitting to a sequence of annotated temporal features.

Deprecated

protocol UpdatableEstimator

An estimator that can be incrementally updated.

protocol UpdatableSupervisedEstimator

A supervised estimator that can be incrementally updated.

protocol UpdatableSupervisedTemporalEstimator

A supervised temporal estimator that can be incrementally updated.

Deprecated

protocol UpdatableSupervisedTabularEstimator

A supervised tabular estimator that can be incrementally updated.

protocol UpdatableTemporalEstimator

A temporal estimator that can be incrementally updated.

Deprecated

protocol UpdatableTabularEstimator

A tabular estimator that can be incrementally updated.

