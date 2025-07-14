

- Create ML Components
-  TabularTransformer 

Protocol

# TabularTransformer

A tabular transformer that transforms a data frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
protocol TabularTransformer : Transformer where Self.Input == DataFrame, Self.Output == DataFrame
```

## Overview

Tabular transformers represent operations on data frames. They modify and operate on values on one or more columns.

## Topics

### Appending

func appending&lt;Other>(Other) -> PreprocessingSupervisedTabularEstimator&lt;Self, Other>

Composes this transformer with a supervised tabular estimator.

func appending&lt;Other>(Other) -> PreprocessingUpdatableTabularEstimator&lt;Self, Other>

Composes this transformer with an updatable estimator.

func appending&lt;Other>(Other) -> PreprocessingTabularEstimator&lt;Self, Other>

Composes this transformer with an estimator.

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTabularEstimator&lt;Self, Other>

Composes this transformer with an updatable supervised estimator.

func appending&lt;Other>(Other) -> some SupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self, Other.Transformer>, Other.Annotation> 

Composes this transformer with a supervised tabular estimator.

func appending&lt;Other>(Other) -> some TabularEstimator&lt;ComposedTabularTransformer&lt;Self, Other.Transformer>> 

Compose this tabular transformer with a tabular estimator.

### Applying and adapting

func appending&lt;Other>(Other) -> ComposedTabularTransformer&lt;Self, Other>

Composes this tabular transformer with another tabular transformer.

func adaptedAsEstimator() -> TabularTransformerToEstimatorAdaptor&lt;Self>

Exposes this tabular transformer as a trivial tabular estimator.

func adaptedAsUpdatableEstimator() -> TabularTransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this tabular transformer as an updatable tabular estimator.

### Transforming

func callAsFunction(DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Performs the transformation on a single input.

### Exporting

func export(to: URL) throws

Exports this transformer as a CoreML model.

func export(to: URL, metadata: ModelMetadata) throws

Exports this tabular transformer as a CoreML model with userInfo.

## Relationships

### Inherits From

- Transformer

### Conforming Types

- ColumnConcatenator
- ColumnSelectorTransformer
- ComposedTabularTransformer
- TreeClassifierModel
- TreeRegressorModel

## See Also

### Tabular components

protocol TabularEstimator

A tabular estimator that creates a transformer by fitting to a data set in a data frame.

protocol SupervisedTabularEstimator

A tabular estimator that creates a transformer by fitting to a data set in a data frame.

struct ColumnSelector

An operation that applies an estimator to a selection of columns.

struct ColumnSelectorTransformer

A transformer that applies a base transformer to specific columns in a data frame.

enum ColumnSelection

A selection of columns from a data frame.

struct ColumnConcatenator

A transformer that concatenates every numerical column in a dataframe into to a shaped array for each row.

struct PreprocessingSupervisedTabularEstimator

A supervised tabular estimator that composes a preprocessing transformer and a supervised tabular estimator.

struct PreprocessingTabularEstimator

An estimator that composes a preprocessing transformer and an estimator.

struct PreprocessingUpdatableSupervisedTabularEstimator

An updatable supervised estimator that composes a preprocessing transformer and an updatable supervised estimator.

struct PreprocessingUpdatableTabularEstimator

An updatable estimator that composes a preprocessing transformer and an updatable estimator.

