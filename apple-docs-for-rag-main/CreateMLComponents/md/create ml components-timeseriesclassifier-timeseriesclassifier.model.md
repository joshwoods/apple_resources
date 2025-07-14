

- Create ML Components
- TimeSeriesClassifier
-  TimeSeriesClassifier.Model 

Structure

# TimeSeriesClassifier.Model

A time-series classifier model.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct Model
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Overview

Note

Only `Float` and `Double` are currently supported as the Scalar type.

## Topics

### Instance Properties

var stride: Int

The number of samples between temporal predictions.

### Instance Methods

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> ClassificationDistribution&lt;Label>

Performs a classification on a shaped array of input features.

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

Decodable Implementations

Encodable Implementations

TemporalTransformer Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Sendable
- TemporalTransformer

  Conforms when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

- Transformer

