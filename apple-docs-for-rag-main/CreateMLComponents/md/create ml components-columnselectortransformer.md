

- Create ML Components
-  ColumnSelectorTransformer 

Structure

# ColumnSelectorTransformer

A transformer that applies a base transformer to specific columns in a data frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct ColumnSelectorTransformer where Base : Transformer, Base.Input == UnwrappedInput?
```

## Topics

### Creating the transformer

init(transformers: [String : Base], columnMapping: [String : String])

Creates a select transformer.

### Getting the properties

var columnMapping: [String : String]

A mapping of input column names to output column names.

var transformers: [String : Base]

A dictionary of column names to transformers.

### Applying a transformation

func applied(to: DataFrame, eventHandler: EventHandler?) async throws -> DataFrame

Performs the transformation on selected columns of the data frame.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Decodable Implementations

Encodable Implementations

TabularTransformer Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
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

