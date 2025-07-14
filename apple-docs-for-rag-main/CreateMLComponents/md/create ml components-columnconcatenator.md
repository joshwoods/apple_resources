

- Create ML Components
-  ColumnConcatenator 

Structure

# ColumnConcatenator

A transformer that concatenates every numerical column in a dataframe into to a shaped array for each row.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct ColumnConcatenator where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint
```

## Overview

The resulting concatenated column contains `MLShapedArray` elements. For example

```
┏━━━┳━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━┳━━━━━━━┳━━━━━━━┳━━━━━━━┓
┃   ┃ label    ┃ price   ┃ rooms ┃ A     ┃ B     ┃ C     ┃
┃   ┃  ┃    ┃  ┃  ┃  ┃  ┃
┡━━━╇━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━╇━━━━━━━╇━━━━━━━╇━━━━━━━┩
│ 0 │ good     │ 850,000 │     4 │     1 │     0 │     0 │
│ 1 │ bad      │ 700,000 │     3 │     0 │     1 │     0 │
│ 2 │ bad      │ 650,000 │     3 │     0 │     0 │     1 │
│ 3 │ good     │ 600,000 │     2 │     0 │     1 │     0 │
└───┴──────────┴─────────┴───────┴───────┴───────┴───────┘
```

would be concatenated as:

```
┏━━━┳━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━┓
┃   ┃ label    ┃ features               ┃
┃   ┃  ┃ > ┃
┡━━━╇━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━┩
│ 0 │ good     │ [850,000, 4, 1, 0, 0]  │
│ 1 │ bad      │ [700,000, 3, 0, 1, 0]  │
│ 2 │ bad      │ [650,000, 3, 0, 0, 1]  │
│ 3 │ good     │ [600,000, 2, 0, 1, 0]  │
└───┴──────────┴────────────────────────┘
```

Non-numerical columns are left in the data frame unchanged. Supported numeric types are `Int`, `UInt8`, `Float`, and `Double`. Arrays and shaped arrays of those types as supported, but every array in a given column must have the same shape and shaped arrays across columns must have the same shape except for the last dimension.

## Topics

### Creating the concatenator

init(columnSelection: ColumnSelection, concatenatedColumnName: String)

Creates a concatenator that concatenates numeric columns into a new column of ML shaped array.

### Getting the properties

var columnSelection: ColumnSelection

The selection of columns to concatenate.

var concatenatedColumnName: String

The name of the concatenated column containing the shaped arrays.

### Applying

func applied(to: DataFrame, eventHandler: EventHandler?) throws -> DataFrame

Combines every numerical column in a data frame into to a shaped array for each row.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

TabularTransformer Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Sendable
- TabularTransformer
- Transformer

## See Also

### Tabular components

protocol TabularTransformer

A tabular transformer that transforms a data frame.

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

struct PreprocessingSupervisedTabularEstimator

A supervised tabular estimator that composes a preprocessing transformer and a supervised tabular estimator.

struct PreprocessingTabularEstimator

An estimator that composes a preprocessing transformer and an estimator.

struct PreprocessingUpdatableSupervisedTabularEstimator

An updatable supervised estimator that composes a preprocessing transformer and an updatable supervised estimator.

struct PreprocessingUpdatableTabularEstimator

An updatable estimator that composes a preprocessing transformer and an updatable estimator.

