

- Create ML Components
-  AnnotatedFeatureProvider 

Structure

# AnnotatedFeatureProvider

An adaptor that converts a regular estimator to a tabular estimator by selecting features and annotations from columns.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct AnnotatedFeatureProvider where Base : SupervisedEstimator, Base.Transformer.Input == UnwrappedInput?
```

## Overview

Tabular estimators use multiple features columns as input. When there is a single column of features, you may use a non-tabular estimator. Do this by combining multiple columns with a `ColumnConcatenator` transformer. Once there is a single column of features, use `AnnotatedFeatureProvider` to specify which column contains the features, which column contains the annotations, and which column should hold the results.

When using `AnnotatedFeatureProvider`, make sure to handle missing values before using a non-tabular estimator that takes non-optional values. This example includes an `OptionalUnwrapper` transformer.

```
let concatenation = ColumnConcatenator(
    columnSelection: .include(columnNames: ["type", "region"]),
    concatenatedColumnName: "features"
)
let regression = AnnotatedFeatureProvider(
    OptionalUnwrapper>().appending(LinearRegressor()),
    annotationsColumnName: "price",
    featuresColumnName: "features",
    resultsColumnName: "result"
)
let task = concatenation.appending(regression)
```

## Topics

### Creating the provider

init(Base, annotationsColumnName: String, featuresColumnName: String, resultsColumnName: String)

Creates an adaptor that converts a regular estimator to a tabular estimator.

### Getting the properties

var annotationColumnID: ColumnID&lt;AnnotatedFeatureProvider&lt;Base, UnwrappedInput>.Annotation>

The annotation column identifier.

typealias Annotation

The annotation type.

var base: Base

The base estimator.

var featuresColumnName: String

The features column name.

var resultsColumnName: String

The results column name.

### Encoding and decoding

func encode(AnnotatedFeatureProvider&lt;Base, UnwrappedInput>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> AnnotatedFeatureProvider&lt;Base, UnwrappedInput>.Transformer

Decodes a previously fitted transformer.

### Fitting

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> ColumnSelectorTransformer&lt;Base.Transformer, UnwrappedInput>

Fits a transformer to a data frame

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

SupervisedTabularEstimator Implementations

UpdatableSupervisedTabularEstimator Implementations

## Relationships

### Conforms To

- Copyable
- Sendable
- SupervisedTabularEstimator
- UpdatableSupervisedTabularEstimator

  Conforms when `Base` conforms to `UpdatableSupervisedEstimator`, `UnwrappedInput` conforms to `Copyable`, `UnwrappedInput` conforms to `Escapable`, and `Base.Transformer.Input` is `UnwrappedInput?`.

## See Also

### Annotations

struct AnnotatedFiles

An annotated files collection.

struct AnnotatedBatch

A batch of annotated examples for fitting a supervised estimator.

struct AnnotatedFeature

An annotated example for fitting a supervised estimator.

struct AnnotatedPrediction

An annotated prediction.

struct DataFrameTemporalAnnotationParameters

Annotation parameters for the dataframe containing temporal annotations.

