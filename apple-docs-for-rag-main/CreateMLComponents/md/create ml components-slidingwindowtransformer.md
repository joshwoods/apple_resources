

- Create ML Components
-  SlidingWindowTransformer 

Structure

# SlidingWindowTransformer

A temporal transformer that groups input elements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct SlidingWindowTransformer where Input : Sendable
```

## Topics

### Creating a transformer

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(stride: Int, length: Int)

Creates a window temporal transformer.

### Getting the properties

let length: Int

The length of a window.

let stride: Int

The number of elements between the start of two consecutive windows.

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) throws -> SlidingWindowTransformer&lt;Input>.WindowSequence

Extracts a window sequence from the input sequence

typealias Input

The input type.

typealias Output

The output type.

struct WindowSequence

An async sequence of windows.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Aliases

typealias OutputSequence

The output async sequence type.

### Default Implementations

TemporalTransformer Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Sendable
- TemporalTransformer

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

struct Downsampler

A temporal transformer that down samples the input stream.

struct VideoReader

A video file reader.

struct TemporalFileSegment

A URL and a time range identifying a specific segment of a time-based (temporal) file.

