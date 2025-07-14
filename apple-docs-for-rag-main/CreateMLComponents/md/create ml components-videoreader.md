

- Create ML Components
-  VideoReader 

Structure

# VideoReader

A video file reader.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct VideoReader
```

## Topics

### Creating the reader

init()

Creates a video reader.

### Reading

static func read&lt;S>(S) async throws -> [VideoReader.AsyncFrames]

Reads a sequence of files as an array of async sequences of video frames.

static func read&lt;S, Annotation>(S) async throws -> [AnnotatedFeature&lt;VideoReader.AsyncFrames, Annotation>]

Reads a sequence of annotated files as an array of annotated async sequences of video frames.

static func readCamera(configuration: VideoReader.CameraConfiguration) async throws -> VideoReader.CameraAsyncBuffers

Reads an async sequence of video frames captured with a video camera.

static func read(contentsOf: URL) async throws -> VideoReader.AsyncFrames

Reads a video file as an async sequence of video frames.

struct AsyncFrames

An async sequence of video frames.

struct CameraAsyncBuffers

An async sequence of video frames.

struct CameraConfiguration

The configuration of the camera to pass to the `readCamera` method.

### Applying

func applied(to: URL, eventHandler: EventHandler?) async throws -> VideoReader.AsyncFrames

Reads a video file as an async sequence of video frames.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

Transformer Implementations

## Relationships

### Conforms To

- Sendable
- Transformer

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

struct TemporalFileSegment

A URL and a time range identifying a specific segment of a time-based (temporal) file.

