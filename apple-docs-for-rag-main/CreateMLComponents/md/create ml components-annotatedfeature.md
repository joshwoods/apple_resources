

- Create ML Components
-  AnnotatedFeature 

Structure

# AnnotatedFeature

An annotated example for fitting a supervised estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct AnnotatedFeature
```

## Mentioned in 

Creating a multi-label image classifier

## Topics

### Creating the feature

init(feature: Feature, annotation: Annotation)

Creates an example with a feature and an annotation.

### Getting the properties

var annotation: Annotation

The annotation.

var feature: Feature

The feature value.

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

struct AnnotatedFeatureProvider

An adaptor that converts a regular estimator to a tabular estimator by selecting features and annotations from columns.

struct AnnotatedPrediction

An annotated prediction.

struct DataFrameTemporalAnnotationParameters

Annotation parameters for the dataframe containing temporal annotations.

