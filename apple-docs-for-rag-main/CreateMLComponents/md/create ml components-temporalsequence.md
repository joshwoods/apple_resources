

- Create ML Components
-  TemporalSequence 

Protocol

# TemporalSequence

Async sequence for temporal features.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol TemporalSequence : AsyncSequence
```

## Topics

### Getting the sequence count

var count: Int?

The number of elements in the sequence if available, calculated nondestructively.

**Required**

### Associating the types

associatedtype Feature

The feature type.

**Required**

## Relationships

### Inherits From

- AsyncSequence

### Conforming Types

- AnyTemporalSequence
- AudioFeaturePrint.FeatureSequence
- AudioReader.AsyncBuffers
- AudioReader.MicrophoneAsyncBuffers
- Downsampler.DownStreamSequence

  Conforms when `Input` conforms to `Sendable`.

- HumanBodyActionCounter.CumulativeSumSequence
- PreprocessedFeatureSequence
- SlidingWindowTransformer.WindowSequence

  Conforms when `Input` conforms to `Sendable`.

- VideoReader.AsyncFrames
- VideoReader.CameraAsyncBuffers

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

struct LinearTimeSeriesForecaster

A time-series forecasting estimator.

struct LinearTimeSeriesForecasterConfiguration

The configuration for a linear time-series forecaster.

struct TimeSeriesForecasterBatches

A sequence of forecaster batches on a time series shaped array.

struct TimeSeriesForecasterAnnotatedWindows

A sequence of forecasting windows on a time series shaped array.

struct TemporalFeature

A temporal feature contains a segment identifier and a feature value.

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

