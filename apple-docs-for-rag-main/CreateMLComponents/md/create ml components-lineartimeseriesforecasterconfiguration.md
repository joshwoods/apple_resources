

- Create ML Components
-  LinearTimeSeriesForecasterConfiguration 

Structure

# LinearTimeSeriesForecasterConfiguration

The configuration for a linear time-series forecaster.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct LinearTimeSeriesForecasterConfiguration
```

## Topics

### Operators

static func == (LinearTimeSeriesForecasterConfiguration, LinearTimeSeriesForecasterConfiguration) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(inputWindowSize: Int, forecastWindowSize: Int)

Creates a configuration.

### Instance Properties

var batchSize: Int

The number of examples in each training batch.

var earlyStoppingIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var earlyStoppingTolerance: Float

The early-stopping tolerance.

var forecastWindowSize: Int

The number of predicted samples.

var hashValue: Int

The hash value.

var inputWindowSize: Int

The number of input samples.

var learningRate: Float

The starting learning rate.

var maximumIterationCount: Int

The maximum number of allowed passes through the data.

var randomSeed: Int?

A seed to generate reproducible results from random operations.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

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

