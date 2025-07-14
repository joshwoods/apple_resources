

- Create ML Components
-  DateFeatureExtractor 

Structure

# DateFeatureExtractor

A time and date feature extractor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DateFeatureExtractor where Scalar : BinaryFloatingPoint
```

## Overview

This transformer takes a Date and extracts floating-point feature values according to the features parameter. Every feature value is roughly between -0.5 and 0.5. All date calculations are based on a Calendar, which defaults to current.

## Topics

### Initializers

init(features: DateFeatures, calendar: Calendar)

Creates a date feature extractor.

### Instance Properties

let calendar: Calendar

The calendar.

let features: DateFeatures

The date and time features.

### Instance Methods

func applied(to: Date, eventHandler: EventHandler?) -> [Scalar]

Extracts features of a particular date.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

Decodable Implementations

Encodable Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
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

struct VideoReader

A video file reader.

struct TemporalFileSegment

A URL and a time range identifying a specific segment of a time-based (temporal) file.

