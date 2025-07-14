

- Create ML Components
-  AnnotatedBatch 

Structure

# AnnotatedBatch

A batch of annotated examples for fitting a supervised estimator.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct AnnotatedBatch where Scalar : MLShapedArrayScalar
```

## Topics

### Initializers

init(features: MLShapedArray&lt;Scalar>, annotations: MLShapedArray&lt;Scalar>)

Creates an annotated batch.

### Instance Properties

var annotations: MLShapedArray&lt;Scalar>

The shaped array of annotations.

var count: Int

The number of examples in the batch.

var features: MLShapedArray&lt;Scalar>

The shaped array of features.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Annotations

struct AnnotatedFiles

An annotated files collection.

struct AnnotatedFeature

An annotated example for fitting a supervised estimator.

struct AnnotatedFeatureProvider

An adaptor that converts a regular estimator to a tabular estimator by selecting features and annotations from columns.

struct AnnotatedPrediction

An annotated prediction.

struct DataFrameTemporalAnnotationParameters

Annotation parameters for the dataframe containing temporal annotations.

