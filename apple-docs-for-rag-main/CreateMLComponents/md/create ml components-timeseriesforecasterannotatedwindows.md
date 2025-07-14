

- Create ML Components
-  TimeSeriesForecasterAnnotatedWindows 

Structure

# TimeSeriesForecasterAnnotatedWindows

A sequence of forecasting windows on a time series shaped array.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TimeSeriesForecasterAnnotatedWindows where Scalar : MLShapedArrayScalar
```

## Overview

A time-series forecaster takes a series of samples and produces a prediction of the next samples. For example the sequence `[1, 2, 3, 4]` could predict `[5, 6]`.

The shape of each feature in the sequence is `[inputWindowSize, featureSize]` and the shape of each annotation is `[forecastWindowSize, annotationSize]`. The sequence will return as many feature-annotation examples as fit in the input. For example an input sequence of size of 10 with an input sample count of 4, a prediction sample count of 2, and a stride of 1 will produce 5 annotated windows:

```
feature: [1, 2, 3, 4], annotation: [5, 6]
feature: [2, 3, 4, 5], annotation: [6, 7]
feature: [3, 4, 5, 6], annotation: [7, 8]
feature: [4, 5, 6, 7], annotation: [8, 9]
feature: [5, 6, 7, 8], annotation: [9, 10]
```

Note that 9 and 10 are never used as features because there would be no annotations for those samples.

## Topics

### Initializers

init(features: MLShapedArray&lt;Scalar>, annotations: MLShapedArray&lt;Scalar>, inputWindowSize: Int, forecastWindowSize: Int, stride: Int, shufflesElements: Bool) throws

Creates a batch sequence.

### Instance Properties

let annotations: MLShapedArray&lt;Scalar>

The original annotations.

let features: MLShapedArray&lt;Scalar>

The original features.

let forecastWindowSize: Int

The prediction sample count.

let inputWindowSize: Int

The input sample count.

var shufflesElements: Bool

A Boolean value indicating whether to shuffle the elements.

var stride: Int

The number of samples between windows.

var underestimatedCount: Int

A value less than or equal to the number of elements in the sequence, calculated nondestructively.

### Instance Methods

func makeIterator() -> TimeSeriesForecasterAnnotatedWindows&lt;Scalar>.Iterator

Returns an iterator over the elements of this sequence.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

### Default Implementations

Sequence Implementations

## Relationships

### Conforms To

- Sendable
- Sequence

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

