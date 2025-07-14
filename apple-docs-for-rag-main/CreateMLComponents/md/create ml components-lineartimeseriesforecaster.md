

- Create ML Components
-  LinearTimeSeriesForecaster 

Structure

# LinearTimeSeriesForecaster

A time-series forecasting estimator.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct LinearTimeSeriesForecaster where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint
```

## Overview

Note

Only `Float` and `Double` are currently supported as the Scalar type. You may get faster training when using `Float`.

## Topics

### Structures

struct Model

A linear time-series forecasting model.

### Initializers

init(configuration: LinearTimeSeriesForecaster&lt;Scalar>.Configuration)

Creates a linear time-series forecaster.

### Instance Properties

let configuration: LinearTimeSeriesForecaster&lt;Scalar>.Configuration

The configuration.

var forecastWindowSize: Int

The number of predicted samples.

var inputWindowSize: Int

The number of input samples.

### Instance Methods

func fitted(to: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws -> LinearTimeSeriesForecaster&lt;Scalar>.Model

Fits a model to a sequence of examples.

func fitted(to: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, validateOn: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws -> LinearTimeSeriesForecaster&lt;Scalar>.Model

Fits a model to a sequence of examples with validation.

func fitted(toWindows: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws -> LinearTimeSeriesForecaster&lt;Scalar>.Model

Fits a model to a sequence of windows.

func fitted(toWindows: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, validateOn: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws -> LinearTimeSeriesForecaster&lt;Scalar>.Model

Fits a model to a sequence of annotated windows with validation.

func update(inout LinearTimeSeriesForecaster&lt;Scalar>.Transformer, with: AnnotatedBatch&lt;Scalar>) async throws -> Scalar

Updates a model with a new batch of examples.

func update(inout LinearTimeSeriesForecaster&lt;Scalar>.Model, withWindows: some Sequence&lt;AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>>, eventHandler: EventHandler?) async throws

Updates a model with a sequence of windows.

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

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- UpdatableSupervisedEstimator

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## See Also

### Time-based components

Creating a time-series classifier

Train a machine learning model to predict the class label of time-series signals.

Creating a time-series forecaster

Forecast future data points by training a machine learning model using historical data.

struct DateFeatures

A set of date and time features.

struct DateFeatureExtractor

A time and date feature extractor.

struct LinearTimeSeriesForecasterConfiguration

The configuration for a linear time-series forecaster.

struct TimeSeriesForecasterBatches

A sequence of forecaster batches on a time series shaped array.

struct TimeSeriesForecasterAnnotatedWindows

A sequence of forecasting windows on a time series shaped array.

struct TemporalFeature

A temporal feature contains a segment identifier and a feature value.

protocol TemporalSequence

Async sequence for temporal features.

struct TemporalSegmentIdentifier

Uniquely identifiers a segment of a temporal sequence.

struct SlidingWindows

A sequence of windows on a time series shaped array.

struct SlidingWindowTransformer

A temporal transformer that groups input elements.

struct Downsampler

A temporal transformer that down samples the input stream.

struct VideoReader

A video file reader.

struct TemporalFileSegment

A URL and a time range identifying a specific segment of a time-based (temporal) file.

