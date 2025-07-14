

- Create ML Components
- LinearTimeSeriesForecaster
-  LinearTimeSeriesForecaster.Model 

Structure

# LinearTimeSeriesForecaster.Model

A linear time-series forecasting model.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Model
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Overview

Note

Only `Float` and `Double` are currently supported as the Scalar type.

## Topics

### Instance Properties

var annotationSize: Int

The number of annotations per sample.

var bias: MLShapedArray&lt;Scalar>?

The bias coefficients.

var featureSize: Int

The number of features per sample.

var forecastWindowSize: Int

The number of prediction samples.

var inputWindowSize: Int

The number of input samples.

var stride: Int

The number of samples between windows.

var weight: MLShapedArray&lt;Scalar>

The linear coefficients.

### Instance Methods

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> MLShapedArray&lt;Scalar>

Performs a prediction on a shaped array of features.

func applied(to: some Sequence&lt;MLShapedArray&lt;Scalar>>, eventHandler: EventHandler?) async throws -> [MLShapedArray&lt;Scalar>]

Performs a prediction on a sequence of input features.

func applied(toWindow: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> MLShapedArray&lt;Scalar>

Performs a prediction on a window of input features.

func export(to: URL) throws

Exports this transformer as a CoreML model package.

func export(to: URL, metadata: ModelMetadata) throws

Exports this transformer as a CoreML model package with user-supplied metadata.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

TemporalTransformer Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- Sendable
- TemporalTransformer

  Conforms when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

- Transformer

