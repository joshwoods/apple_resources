

- Create ML Components
-  DateFeatures 

Structure

# DateFeatures

A set of date and time features.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DateFeatures
```

## Overview

The choice of features for a particular task depends on the relevance of different date and time components. For example a dataset of weather data may require hour and day-of-year features, while a dataset of workout metrics may require second, hour, and weekday features.

## Topics

### Initializers

init(rawValue: Int)

Creates a feature from a raw value.

### Instance Properties

var rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let day: DateFeatures

A feature representing the day within the month.

static let dayOfYear: DateFeatures

A feature representing the day within the year.

static let hour: DateFeatures

A feature representing the hour within the day.

static let minute: DateFeatures

A feature representing the minute within the hour.

static let month: DateFeatures

A feature representing the month within the year.

static let second: DateFeatures

A feature representing the second within the minute.

static let weekOfMonth: DateFeatures

A feature representing the week within the month.

static let weekOfYear: DateFeatures

A feature representing the week within the year.

static let weekday: DateFeatures

A feature representing the weekday.

### Default Implementations

Equatable Implementations

OptionSet Implementations

RawRepresentable Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Time-based components

Creating a time-series classifier

Train a machine learning model to predict the class label of time-series signals.

Creating a time-series forecaster

Forecast future data points by training a machine learning model using historical data.

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

struct VideoReader

A video file reader.

struct TemporalFileSegment

A URL and a time range identifying a specific segment of a time-based (temporal) file.

