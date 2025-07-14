

- Create ML Components
-  PreprocessedFeatureSequence 

Structure

# PreprocessedFeatureSequence

An asynchronous sequence of eagerly stored temporal features.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct PreprocessedFeatureSequence
```

## Overview

This sequence eagerly stores the results of preprocessing a temporal estimator.

## Topics

### Creating a sequence

init&lt;S>(S) async throws

Creates an asynchronous sequence of stored temporal features.

### Getting the properties

var count: Int?

The stored temporal feature count.

var features: [TemporalFeature&lt;Feature>]

The stored temporal features.

### Creating an iterator

func makeAsyncIterator() -> PreprocessedFeatureSequence&lt;Feature>.AsyncIterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

### Type Aliases

typealias Element

The type of element produced by this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence
- TemporalSequence

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

struct VideoReader

A video file reader.

