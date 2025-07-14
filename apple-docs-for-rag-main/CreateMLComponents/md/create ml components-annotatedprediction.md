

- Create ML Components
-  AnnotatedPrediction 

Structure

# AnnotatedPrediction

An annotated prediction.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
struct AnnotatedPrediction
```

## Topics

### Creating an annotated prediction

init(prediction: Prediction, annotation: Annotation)

Creates an annotated preditction.

### Getting the properties

var annotation: Annotation

The ground truth annotation.

var prediction: Prediction

The predicted value.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Annotations

struct AnnotatedFiles

An annotated files collection.

struct AnnotatedBatch

A batch of annotated examples for fitting a supervised estimator.

struct AnnotatedFeature

An annotated example for fitting a supervised estimator.

struct AnnotatedFeatureProvider

An adaptor that converts a regular estimator to a tabular estimator by selecting features and annotations from columns.

struct DataFrameTemporalAnnotationParameters

Annotation parameters for the dataframe containing temporal annotations.

