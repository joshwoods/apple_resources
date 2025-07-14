

- Create ML Components
-  ColumnSelector 

Structure

# ColumnSelector

An operation that applies an estimator to a selection of columns.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct ColumnSelector where Estimator : Estimator, Estimator.Transformer.Input == UnwrappedInput?
```

## Overview

This estimator applies a non-tabular estimator to a selection of columns. Here’s an example of normalizing numeric values within each column using a StandardScaler:

```
let numericalScaling = ColumnSelector(
    columns: ["volume", "price"],
    estimator: NumericImputer(.mean)
        .appending(StandardScaler())
)
```

In most cases, an inputer must handle missing values.

## Topics

### Creating the selection

init(columns: [String], estimator: Estimator)

Creates a select operation with an estimator.

init(ColumnSelection, estimator: Estimator)

Creates a select operation with an estimator.

init&lt;T>(ColumnSelection, transformer: T)

Creates a select operation with a transformer.

### Getting the properties

var columnSelection: ColumnSelection

The column selection strategy.

var estimator: Estimator

The estimator to use on each column.

### Encoding and decoding

func encode(ColumnSelector&lt;Estimator, UnwrappedInput>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> ColumnSelector&lt;Estimator, UnwrappedInput>.Transformer

Decodes a previously fitted transformer.

### Fitting a transformer

func fitted(to: DataFrame, eventHandler: EventHandler?) async throws -> ColumnSelector&lt;Estimator, UnwrappedInput>.Transformer

Fits a transformer to a data frame

typealias Input

typealias Output

typealias Transformer

The transformer type created by this estimator.

### Default Implementations

TabularEstimator Implementations

UpdatableTabularEstimator Implementations

## Relationships

### Conforms To

- Copyable
- Sendable
- TabularEstimator
- UpdatableTabularEstimator

  Conforms when `Estimator` conforms to `UpdatableEstimator`, `UnwrappedInput` conforms to `Copyable`, `UnwrappedInput` conforms to `Escapable`, and `Estimator.Transformer.Input` is `UnwrappedInput?`.

## See Also

### Tabular components

protocol TabularTransformer

A tabular transformer that transforms a data frame.

protocol TabularEstimator

A tabular estimator that creates a transformer by fitting to a data set in a data frame.

protocol SupervisedTabularEstimator

A tabular estimator that creates a transformer by fitting to a data set in a data frame.

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

